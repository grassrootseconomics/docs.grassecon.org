# SPROUT Swap Loan Terms (Sign-at-Swap)
**Version:** v0.1  
**Last updated:** 24 Jan 2026  

**Pool / Steward:** Steward / Name of Pool (“**Pool**”)  
**You / Wallet holder:** the person controlling the signing wallet (“**Swapper**”)

---

## 1) Acceptance and binding effect
By clicking **“Sign & Swap”** (or equivalent) and signing the wallet message, you enter into a binding agreement with the Pool for this specific swap (a “**Swap Loan**”). You agree that your electronic signature, the signed message, and the on-chain transaction record may be used as evidence of your agreement and the Swap Loan terms you accepted.

---

## 2) Transaction Terms incorporated by reference
The following transaction-specific terms shown to you at signing time (and/or included in the signed message and on-chain call) form part of this agreement (“**Transaction Terms**”):

- **Input Asset (Collateral / Loan Voucher):** \[token/voucher/asset] + amount  
- **Output Asset (Advance):** \[token/cash-equivalent/asset] + amount  
- **Repayment Amount:** \[equal to Output Amount + disclosed fee]  
- **Due Date:** \[timestamp/date; default: 1 year from signing unless stated otherwise]  
- **Fees (if any):** \[must be shown before signing]  
- **Pool contract / pool ID:** mustardseedlings@grassecon.org  
- **Swap nonce / quote ID:** \[given at time of swap]  
- **Full Value (for this Swap Loan):** the value assigned to the Collateral in the Transaction Terms at the moment you sign (the “**Full Value**”).

If there is any conflict between these Terms and the Transaction Terms, the Transaction Terms you signed control for that Swap Loan.

---

## 3) What this swap is (always a 0% interest loan; creditor may change)
This swap creates a **0% interest loan advance** from the Pool to you, secured by your collateral.

- **(a) Advance.** The Pool delivers the Output Asset to you (the “**Advance**”).  
- **(b) 0% interest.** Interest is **0%** unless the Transaction Terms explicitly state otherwise.  
- **(c) Characterization (intent).** The Advance is a repayable loan/advance and is not intended as income or payment for services at the time of receipt; settlement occurs only upon repayment/redemption.  
- **(d) Your obligation is always a loan obligation.** By signing, you acknowledge you have borrowed the Advance and you owe repayment of the Repayment Amount by the Due Date.  
- **(e) Transferability.** You agree that the Pool may transfer/assign the loan claim to another party by transferring the Collateral/Loan Voucher. If that happens, you will owe the same loan obligation to the current holder (the “**Holder**”) instead of the Pool. The loan does not end; only the lender/creditor changes.

---

## 4) Collateral transfer to the Pool; Pool may use it anytime
- **(a) You pledge/transfer collateral.** You transfer the approved Input Asset (Voucher) to the Pool as collateral and loan evidence for this Swap Loan.  
- **(b) Pool may use/transfer collateral at any time.** You expressly agree the Pool may hold, swap, transfer, lend, sell, auction, or otherwise dispose of the collateral at any time, including before and after the Due Date, according to Pool rules and on-chain functionality.  
- **(c) The collateral is also the “Loan Voucher.”** If the collateral is your own voucher (or a voucher linked to your performance), you agree it may function as a transferable record of the loan claim.  
- **(d) No right to demand return if transferred.** If the Pool transfers out the collateral, you understand it may no longer be possible to return it to you, because it may now be held by a Holder as part of the loan claim.

---

## 5) When your debt to the Pool ends vs. when your loan obligation ends (assignment clarity clause)
This section is the key “clarity clause.”

### (a) Your loan obligation continues until repaid/redeemed
Your obligation to repay the Repayment Amount continues until it is fully settled through repayment/redemption as defined in Section 6. It does not end just because collateral moves.

### (b) Who you owe can change (assignment)
If the Pool transfers out your collateral (your voucher), you agree that the Pool is assigning the right to receive repayment/redemption of your loan (the “**Loan Claim**”) to the recipient/Holder to the extent of the Full Value transferred.

- From that moment, you no longer owe the Pool for the assigned portion, because the Pool is no longer the lender for that portion.  
- Instead, you owe the same loan obligation for that portion to the Holder.

### (c) Partial transfer-out
If only part of your collateral is transferred out, then only that portion of the Loan Claim is assigned to the Holder, and you continue to owe the Pool for any portion not assigned.

### (d) On-chain notice and proof
You agree that on-chain records (transaction hash, events, and state changes) are conclusive proof of:

- whether your collateral was transferred out,  
- the timing of the transfer, and  
- who the current Holder is (or the address that controls the collateral), and therefore who is entitled to receive repayment/redemption.

### (e) No double-claims
You are not required to pay the same portion twice. Paying/redeeming the correct current Holder as shown by on-chain records discharges that portion of the loan.

---

## 6) How the loan can be repaid (repayment or redemption at Full Value)
This applies whether the lender is the Pool or a Holder.

### (a) Two permitted settlement methods (as chosen by the lender/Holder, per voucher terms)
- **Repayment in approved assets:** you repay the Repayment Amount (or remaining balance) in the approved settlement asset(s) specified in Transaction Terms; **or**  
- **Redemption/Performance at Full Value:** if the collateral is your voucher, you repay by honoring the voucher at Full Value through your offered goods and/or services when requested by the current Holder, consistent with the voucher’s disclosed redemption terms.

### (b) Standing obligation to accept your own voucher at Full Value
You agree that any current Holder of your voucher has the right to request redemption, and you must accept your voucher at Full Value as payment toward your offered goods/services, subject only to:

- legality and safety, and  
- any clear, pre-existing voucher redemption terms disclosed in the voucher itself (what is redeemable, where, and within what time window).

### (c) No refusal / no discounting
You will not refuse redemption, delay unreasonably, or apply a discount below Full Value solely because the voucher passed through the Pool or because the Pool assigned the Loan Claim.

### (d) Redemption process + completion (to prevent double spending)
A Holder redeems by:

1. presenting the voucher ID/record and their delivery address/contact method, and  
2. making a redemption request via \[on-chain call / app request / written notice method].

You must fulfill redemption within **\[X days]** unless the voucher terms specify another window.

**Redemption completion rule (required):**  
To mark repayment complete for that redeemed amount, the Holder must send the Voucher to your designated redemption address (or a burn/cancel address) as specified by the system. Once that on-chain transfer/burn occurs, that redeemed portion is treated as repaid and cannot be claimed again.

### (e) Failure to redeem = default
If you fail to redeem at Full Value when properly requested, that is a Default under Section 7.

**Plain-language summary:** this is always a loan. Your debt can be transferred from the Pool to a Holder by assignment. When a Holder presents your voucher, you repay the loan by providing goods/services at Full Value (or by paying in approved settlement assets), and redemption is completed when the voucher is returned/burned on-chain.

---

## 7) Default and enforcement
You are in Default if any of the following happen:

- **Nonpayment:** you fail to repay any due amount by the Due Date (plus any grace period in Transaction Terms) to the current lender (Pool or Holder).  
- **Non-redemption:** you fail to redeem your voucher at Full Value when properly presented by a Holder under Section 6.  
- **Fraud/invalid collateral:** the collateral you provided is fake, double-pledged, or you lacked authority to transfer it.  
- **Other material breach** of these Terms.

Upon Default, the Pool and/or the current Holder (as applicable and as allowed by pool rules and law) may:

- enforce against collateral (if any remains held by the enforcing party);  
- pursue repayment of the outstanding loan amount;  
- use on-chain remedies (limiters/registries/enforcement functions); and/or  
- take off-chain action where lawful.

---

## 8) Steward encouragement and practical payoff pathway (non-binding)
Pool stewards may encourage people to acquire your voucher from the Pool (for example by swapping stablecoins or approved vouchers) and then redeem it for your goods/services. You understand this is a common pathway for loan settlement: the Pool gets replenished by incoming assets, and the Holder receives your goods/services.

This encouragement is not a guarantee that any particular person will acquire or redeem your voucher.

---

## 9) On-chain records, electronic signatures, and evidence
You consent that the signed wallet message, transaction call data, events, and resulting state changes are a reliable record of your intent and agreement, and may be used as evidence.

---

## 10) Your representations
By signing, you represent that:

- you control the signing wallet and have authority to agree;  
- you own/are authorized to transfer the collateral;  
- you understand the Due Date, Repayment Amount, and that your loan obligation can be assigned to a Holder;  
- you agree to redeem your voucher at Full Value for any Holder under Section 6.

---

## 11) Disclosures and risks
You acknowledge:

- values/limits/fees are set by Pool registries and can change;  
- blockchain transactions are final;  
- asset values and liquidity can change;  
- if your voucher is transferred out, you may owe repayment/redemption to a Holder even if you would have preferred to repay the Pool directly.

---

## 12) Privacy and public data
Blockchain transactions are public and permanent; your address and activity may be visible.

---

## 13) Governing law and disputes
Unless Transaction Terms specify otherwise, these Terms are governed by the laws of Kenya, with disputes resolved by \[Courts of Kenya / Arbitration in Nairobi] per Pool policy.

---

## 14) Severability
If part of these Terms is unenforceable, the rest remains effective.

---

## Signature statement shown at swap time (short “I agree” text)
By signing, I agree: (1) the Pool advances me the Output Asset as a 0% interest Swap Loan, secured by my Input Asset; (2) the Pool may use/transfer my collateral at any time; (3) transferring my voucher collateral does not end the loan— it assigns the lender’s right to repayment/redemption to whoever holds it, so I then owe the Holder; (4) I must redeem my voucher at Full Value for any Holder who presents it (or repay in approved settlement assets), and redemption is completed when the voucher is returned/burned on-chain; and (5) my wallet signature and on-chain records prove this agreement.

