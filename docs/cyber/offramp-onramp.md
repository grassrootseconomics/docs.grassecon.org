# Offramp & Onramp (M-PESA)

This short guide explains how to off-ramp (convert stablecoins to M-PESA cash) and on-ramp (receive stablecoins from an M-PESA push) using M-PESA via USSD or other wallets.

- Supported assets: cUSD, USDT, USDC

## USSD offramp

1. On your USSD send menu, enter the recipient as `mpesa`.
2. Enter the amount. The recommended minimum is 0.3 cUSD/USDT/USDC.
3. You should receive a confirmation message within ~1 minute.

## Offramp using another wallet

1. Ask an admin or staff member to link your wallet to your phone number.
2. Send the amount to the recipient address: `mpesa.sarafu.eth` (`0x8005ee53E57aB11E11eAA4EFe07Ee3835Dc02F98`).
3. You should receive a confirmation message within ~1 minute.

## Onramp

1. Request an admin or staff member to initiate an M-PESA push/prompt for the agreed amount and stablecoin.
2. When you receive the M-PESA prompt, enter your M-PESA PIN to complete the push.
3. You should receive a confirmation message within ~1 minute. Verify your on-chain balance or wait for a Sarafu SMS confirmation.

## Check and contact

- If the transaction doesn't appear after a few minutes, check your wallet balance on-chain and any SMS confirmations.
- For unresolved issues, contact a staff member and provide:
  - Transaction time, amount, and asset (cUSD/USDT/USDC)
  - Sending/receiving address or phone number
  - Any error messages or USSD responses
