# Smoke Testing Proceedure

## Setup

1. via Phone
    1. Dial ```*483*061#``` This is the testing code in Kenya 

### Setup account


1. Choose language
    1. Ensure that you can goto end of Language list and back

You will get a message asking if you agree to the terms and condition
and another telling you your account has been setup and to start again by dialing the code.

1. Ensure you have 0 vouchers
1. Check menu looks like:

    ```Jim12a Balance: 130 RIBA```
 	```1: Send```
    ```2: Swap```
    ```3: My Vouchers```
    ```4: My Account```
    ```5: Help```

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


### Change Voucher
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
    
    ```5. My shortcode```
    
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

