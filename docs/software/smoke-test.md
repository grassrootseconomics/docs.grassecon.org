# Smoke Testing Proceedure

## Setup

1. via Command Line USSD Menu (CLI, Bypass AfricasTalking)

    Setup `cic-stack/cic-ussd`:

    *assumes you are using a unix environment*
    ```bash```
    
    ```git clone https://gitlab.com/grassrootseconomics/cic-internal-integration.git```
    
    ```cd apps/cic-ussd```
    
    ```python3 -m venv .venv```
    
    ```source .venv/bin/activate```
    
    ```pip install -r requirements.txt --extra-index-url=https://pip.grassrootseconomics.net```

    2. Use the CLI

    *assumes you are in the cic-stack/apps/cic-ussd folder*
    
    ```bash```
    
    ```USSD_SERVICE_CODE=*483*061# python cic_ussd/runnable/client.py --host ussd.grassecon.net --port 443 -c $(pwd)/config 254700123456```

    *alternatively, the `cic-ussd-client` package is also available in [ge-dev](https://gitlab.com/grassrootseconomics/ge-dev)*

1. via Phone
    1. Dial ```*483*061#``` This is the testing code in Kenya 

1. via Telegram
    1. Goto @sarafutest_bot and type ```/start```

### Setup account
Once you have been able to do one of the options above for setup. You will get a message telling you your account has ben setup and to start again.

1. Choose language
    1. Ensure that you can goto end of Language list and back
1. Ensure you got 5 SRF tokens
1. Check menu looks like:

    ```Balance 5 SRF```
    
    ```1. Send```
    
    ```2. My Sarafu```
    
    ```3. My Account```
    
    ```4. Help```

### Send

1. Send to registered number
    1. Verify both parties get a receipt SMS 
    1. Check the balance of each user to verify the send happened correctly
    1. Send Fractional units like 0.6 SRF
    1. Use the wrong PIN to send once, then use the correct pin
1. Recieve SRF from another user
1. Send from an account while having insufficient balance
    1. Make sure the error message is understandable
1. Send to number not registered
    1. Verify that the person sent to gets an upselling message


### Change Token
1. Receive a different token than SRF (e.g. FOO)
1. goto My Sarafu Menu and ensure it looks like:

    ```Choose a number or symbol from your balances:```
    
    ```1. SRF 1.4```
    
    ```2. FOO 148.0```
    
    ```0. Back```
    
    ```11. Next```
    
    ```00. Exit```
    
1. Change to another token (e.g. FOO)
    1. Ensure that you can goto end of Language list and back
1. Send that token to someone else
    1. Ensure the receipt messages are ok
    1. Check Statment to ensure it is ok

### My account

1. Goto My Account from main menu
1. Check menu looks like:

    ```My account```
    
    ```1. My profile```
    
    ```2. Change language```
    
    ```3. Check balance```
    
    ```4. Check statement```
    
    ```5. PIN options```
    
    ```0. Back```

1. Enter your profile information under My Profile
   1. Ensure that all the information was set correctly
   1. Send a transaction to someone and make sure that the receipt shows your name
1. Change language
    1. Ensure you can click next several times and back
    1. Ensure that other menus work properly in that language.
        1. Note which language are are choosing for the smoke test report
1. Check Statment
    1. Ensure it reflects your last few transactions
1. Check Balance
    1. Ensure it reflects your last few transactions


### Pin Options
1. Goto Pin Options under My Account
1. Check menu looks like:

    ```Pin options```
    
    ```1. Change my PIN```
    
    ```2. Reset other PIN```
    
    ```3. Guard my PIN```
    
    ```0. Back```
    
1. Change your pin
    1. Ensure you can send a transaction with new pin
1. Set a Guardian (Guard my pin)
    1. and ensure the guardian can reset your pin
    1. Use the wrong PIN to send 3 times
        1. ensure your account is locked
        1. ensure the guardian can reset your pin
    1. Remove a Guardian and ensure they can't reset your pin
1. Have somone set you as their guardian
    1. Reset their pin
    1. Ensure they can make a transaction

### Help
1. Correct helpline 0757628885


## Extra Tests

### Analysis dashboard

#### Dependencies
- [cic-data-golang](https://gitlab.com/grassrootseconomics/cic-data-golang)

1. Goto graphana website .....<>?
1. Adjust filters to be able to see new tokens added.
1. Validate some transactions you just made are shown there.
1. Download a CSV of the most recent transactions and users

### User info

#### Dependencies

- [clicada](https://git.grassecon.net/grassrootseconomics/cic-staff-installer)

1. Use CLICADA to verify the transaction history for a user is correct - compare to mini statments on USSD
1. Choose Another 2 users and verify their balance on the old Sempo system and new system

### Token creation

#### Dependencies

- [cic-cli](https://gitlab.com/cicnet/cic-cli)
- [cic-internal-integration](https://gitlab.com/grassrootseconomics/cic-internal-integration)
- [eth-erc20](https://gitlab.com/cicnet/eth-erc20) | [erc20-demurrage-token](https://gitlab.com/cicnet/erc20-demurrage-token)

1. Command Line: Create a new token with demurrage, name, location, description (try a demurage of 2% per minute and a suply of one million to see the effect on the sink account). Ensure the Sink account is accessible from USSD.
1. Send thse tokens to a user and verify they can use them on USSD

### Batch transfer 

#### Dependencies
- [sendscript](https://gitlab.com/chaintool/chaind-eth/-/tree/lash/sendscript)

1. Create a CSV list of users and send them each some tokens in batch
1. Ensure the users get the correct amount of tokens

