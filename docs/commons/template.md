# **Grassroots Economic Commons Agreement Template (GECAT) v1.22 (en)**


## **About**

This template for general implementation defines a viable Economic Commons as an open association of people and organizations, where mutually defined Instruments are utilized by General Members who jointly oversee essential Core Service Providers as active stewards, subject to Guardians as passive custodians with protective governance rights of arbitration and final veto. All capitalized terms as well as Aims, Principles, Jurisdiction, Definitions, Organization and Notices are defined in this template.


## **Aim**

Community creation and maintenance of Instruments for inclusive well-being.


## **Principles**

The core Principles of an Economic Commons include the following Values:



1. **Care for People** – collaboration and vision driven care for oneself and others’ well-being and happiness 
2. **Care for the Environment** - support environmental protection and regeneration,  minimize use of finite resources for economic activity, ecosystem management approach to farming and business development.
3. **Equity** - affordable and secure access to Instruments, land, resources, knowledge & care for members from different backgrounds, age, gender and religion. 
4. **Reciprocity** – mutual sharing of risk, cost and surplus
5. **Non-Dominance** - no person or association to have dominant rights over any other person or association’s resources like data, finances, intellect, materials and freedom. 
6. **Resilience** - ensure the continuation of community based systems /commons and prepare for economic, political, climate and other shocks

Note that each Association of Member’s signing such an Agreement should be specific with how these Values are incorporated into objective and measurable Principles and Good Practices.


## **Jurisdiction**



1. An Economic Commons, as an associative and participatory Agreement, transcends jurisdiction and is tax transparent
2. Everything in this Agreement is consistent with national law.
3. Any usage of Instruments are between willing Members who must satisfy themselves that usage is lawful in their jurisdiction
4. Data may be shared internationally between Members in different jurisdictions


## **Instruments**


### **Ledger**

A Ledger is an Instrument maintained by Core Service Providers that acts as a Instrument registry and execution system with the following properties:



1. **Instruments** are agreements or contracts created and used by willing Members.
2. **Publishing**: Any Instrument must be Published on a Ledger to be considered valid. To Publish an Instrument it must be encoded into a form that is readable and executable on the Ledger.
3. **Management**: A Ledger is managed by Core Service Providers or agreements between Members and external Ledger service providers. 
4. **Issuer: **The issuer of an Instrument is an individual Member or association of Members who agreed in writing to be joint and severally liable for an Instrument that is Published on a Ledger.


### **Voucher**

**Voucher (Bilateral Instrument)** – a promise denominated in an agreed upon Unit of Account issued and accepted in exchange for money or in-kind and representing an assignable credit obligation of the Issuer. The following are properties of Vouchers:



1. Redemption Policy: If the acceptor/final holder of the Voucher presents it in payment to the Issuer, for goods or services supplied, it _must_ be accepted in payment. Vouchers are only redeemable for payment of the Issuer's products and _cannot be redeemed for cash_.
2. Digital Representation: The Voucher is digital and defined on a secure and immutable public Ledger, where members hold accounts. 
3. Transparency: All Instruments definitions and their usage, as well as all Member accounts are transparent to the public and considered non-confidential.
4. Divisibility: Vouchers can be divided to a specified precision, as determined by the Issuer at the time of Publishing on the Ledger. This means that the holder of one Voucher can send a portion of the Voucher to another member, with the precision specified as a number of digits of precision by the Issuer.
5. Name and Symbol and Contract Address: Each Voucher must have a name and symbol specified by the Issuer, and a unique Contract Address (public key).
6. Contact Information: The Voucher must include contact information for the Holder to know how to redeem the Voucher as payment for the Issuer's products. The Issuer must keep this information accurate and up-to date.Unit of Account: Standard unit of measure for value in exchange. Each Voucher issued by a Member should specify a Unit of Account.
    1. Example: 1000 SRF Vouchers can be said to be redeemable by the Issuing Member for 1000 Kenyan Shillings worth of the Issuer’s services.
7. Expiration: Vouchers may have a specified expiration date or an expiration rate. 
    2. Expiration Rate: For example, a Voucher with an expiration rate of 2% per month would result in a holder having 98 Vouchers at the end of the month, if the holder had 100 Vouchers at the beginning of the month.
    3. Expiration Date: For example a Voucher with an expiration date of one month would result in a holder having 0 usable Vouchers at the end of the month, if the holder had 100 Vouchers at the beginning of the month.
8. Sink Account and Issuance Period: Expired Vouchers will accrue in a specified Ledger account determined by the Issuer after a specified Issuance period. This means that the balance of Vouchers in the Sink Account will increase by the sum of expired Vouchers, after the Issuance Period.
9. Supply: The supply of Vouchers may be increased or destroyed by vote of the Issuers. The supply of Vouchers shall always be based on the Issuer's capacity to redeem them as payment for their products within the specified expiration.
10. Fungibility: Each Voucher is fungible with the vouchers issued under that same contract, meaning that it is interchangeable and mixable with them. An account holding multiple identical Vouchers would display the sum of their quantity as their Voucher Balance minus any expired Vouchers.
11. Bearer Instrument: The Voucher is a “digital bearer instrument”, meaning that anyone holding the access (private) key to the holder's Ledger account is considered the owner of the Voucher or Vouchers in that account. Note that Members may share keys.
12. No Liability for loss or theft: The Issuing or Publishing members are not liable for lost or stolen Instruments or Accounts. 
13. Utility: The Voucher is not marketed or sold by Members as an investment product. It confers no additional rights or benefits beyond the redemption for the Issuer's products.
14. Liability: The Voucher is a credit obligation with joint and several liability of the Issuer. This means that the Issuers are collectively and individually responsible for fulfilling the obligation of the Voucher. A Voucher issued by a group of Issuers is called a Community Asset Voucher.
15. Finality: Once published and registered on the Ledger certain Immutable Information cannot change while Mutable Information can be changed by Voucher Contract Manager.
    4. Immutable Information includes:
        1. Name, Symbol
            1. Expiration dates and rates
            2. Re-issuance period
            3. Precision
            4. Contract Address* (public Key)
            5. Unit of Account*
            6. Description*
            7. Issuer Name*
            8. Namespace*= An domain for which to register the Voucher.
            9. Proofs* (media files, hashes or attachments)
            10. Version number*
            11. Image* (optional logo)
            12. Address of Mutable Information (derived)*
            13. Valid from* (date that the contract was published)
            14. Valid until* (date that the information is considered outdated)
        2. Mutable Information* includes:
            15. Voucher Contract Manager (public key)
            16. Voucher supply (via minting or burning)
            17. Sink address
            18. Contact information*
            19. Name, phone number, email, location, country
            20. Signers (who attest to the certificate information being connected to the Voucher)
        3. (*) Note that all the above information is data stored and registered on a Certificate which is published on the Ledger
16. Voucher Contract Management: The Voucher Contract (Smart contract) registered and published on the Ledger has a Manager that can edit the Mutable Information in the Voucher Contract. The default Manager is the Member that published the contract and who may transfer Management to any Account on the Ledger and also remove themselves as an Manager. Management can be transferred to a Smart Contract that enables different forms of voting etc.


### **Certificate**

**Certificate (Unilateral Instrument)** – an attested to data object that may be accepted by another Member. A Certificate is similar to a University Diploma in which the University makes a claim (an attestation) that a Student has passed their coursework. The following are properties of Certificates:



1. Attestation: Certificates represent collectible attestations to data such as Voucher usage or capacity to perform services. Vouchers as well as Members can be Certified by other Members, for various roles, services, accomplishments and so on. The certification is an attestation by a Member or Members for another Member or Instrument. Note that in the example of a Voucher Instrument some Immutable and Mutable data is stored or referenced to on a Certificate (denoted with a (*).
2. No Obligation: There is no obligation on the Issuer of a Certificate to accept or redeem it.
3. Finality: Once published and registered on the Ledger certain Immutable Information cannot change while Mutable Information can be changed by a Certificate Publisher.
    1. Specification: (TBD)
4. Certificate Contract Management: The Certificate Contract (Smart contract) registered and Published on the Ledger has a Manager that can edit the Mutable Information in the Certificate Contract. The default Manager is the Member that published the contract and who may transfer Management to any Account on the Ledger and also remove themselves as an Manager.
5. Revocation or Expiration: Attestation for a certificate can expire and or be revoked, and the history of attestation must be preserved on the Ledger.
6. Acceptance or Denial: Whomever is holding the Private Key to the public address that is being attested about can choose to accept, deny and comment on the Attestation.
7. Finality: Once published and registered on the Ledger, the Immutable Properties of the Certificate cannot be changed.


## **Organization**


### **Membership**

A Member of an Economic Commons is an individual person, organization or an association of Members with a common purpose, who ratify and Implement an Economic Commons it or use implemented Economic Commons Instruments as per their local needs

There are three Member **Classes** defined below, with the following rights and obligations:


#### **General Members**



1. Right to utilize all Economic Commons-defined Instruments
2. Right to hold or delegate custodianship of Ledger Accounts and Instruments
3. Right to hold multiple Accounts and Instruments in the Ledger
4. Right to vote on the usage of their issued Instruments in a Community Fund
5. Right to view and inspect all Accounts and Instrument kept on the Ledger
6. Obligation to report Members that don't comply to this Agreement or local laws
7. Obligation to certify Core Service Providers
8. Obligation to register any Instrument or Instrument usage on the Ledger and keep any relevant information up to date.
9. Obligation to contribute in money or in-kind the agreed upon development and operating costs of the Core Services as defined in **Service Agreements** under this Economic Commons Agreement
10. Obligation to hold a means of secure identification (such as a private key) in order to interact with a Ledger
11. Obligation to demonstrate technical and management capabilities and capacity to meet Instrument and other appropriate standards.


#### **Core Service Providers**

Provide essential service for the Economic Commons.



1. Technical: \

    1. Secure Member account and shared Instrument on registries (herein called the “Ledger”):
    2. Track and report all usage of all Member account and Instruments, securely and immutably
    3. Provide communications interfaces (such as software that allows interaction with the Ledger - herein called Wallets)
    4. Right to Publish Instruments on the Ledger on behalf of Members when given custodian shop of a Members private Key.
    5. Right to receive agreed development and operating costs and an agreed production share in respect of Core Services
    6. Right to use and migrate custodial Member Accounts and Instruments to an appropriate Ledger
    7. Obligation to maintain an open source software code base under AGPL3.0 for any Core Services and Agreements
    8. Obligation to operate the servers and various micro-service related to Core Services
    9. Obligation to hold and secure granted Member data and intellectual property jointly in common
    10. Obligation to provide Members access to their Ledger accounts and shared Instruments
    11. Obligation to provide a means of a secure identification to Members in order to interact with a Ledger
    12. Obligation to all Member accounts, data and shared Instruments are recorded in unique time order in the Ledger
    13. Obligation to utilize Ledgers that are secure and resistant to security breaches and loss of data
2. Social: \

    14. Support and sharing of knowledge regarding the Agreement's implementations, Instruments as well as Member rights and obligations
    15. Right to make available non-confidential Member and Instrument data to the general public
    16. Right to make available non-confidential Member and Instrument data to the general public
    17. Obligation to provide training and education
    18. Obligation to administer Member service agreements
    19. Obligation to ensure confidential data privacy and public information transparency
    20. Obligation to oversee quality standards
3. Legal: \

    21. Right to assign an auditor to assess any Member Instruments
    22. Right to suspend services and remove Wallet access for Non-Performing Members
    23. Right to assign arbitrators for the mediation of disputes
    24. Obligation to provide Due Diligence, audits and arbitration of disputes for Members in relation to usage of Instruments and this Agreement.
    25. Obligation to ensure that Instruments are binding on Members when registered in the Ledger and inline with this Agreement


#### **Guardians**



1. Right to develop, design, raise resources and implement an Economic Commons
2. Right of final veto on behalf of Members generally in respect of amendments to an Economic Commons agreement incompatible with the Aim and Principles
3. Obligation to arbitrate in the management of Class Agreements and Admissions as described below
4. Obligation to arbitrate disputes of Members in relation to Aim and Principles
5. Obligations to call annual membership meetings, keep records, call meeting to make decisions that serve the aims and principles of the Economic Commons


### **Class Agreements and Admissions**



1. Members may participate in more than one Member Class. E.g. A Core Service Provider can also be a General Member and develop a Voucher redeemable for their services
2. Any person or organizations holding a Ledger-account or whom utilizes Instruments is considered a General Member
3. Mutual agreements between Members define standards, rights and obligations
4. **Non-Performance:** should a Member be unable or unwilling to uphold their obligations or honor stated commitments they should immediately Issue a Certificate to attest to the situation and report to any Instrument Publishers and Members holding their Instruments. Such a Member will be designated as Non-Performing subject to the following:
    1. any material shortfall in commitments or obligations by Members individually or collectively shall be made good following review and recommendations by the Service Provider and subject to the agreement of Members generally.
5. **Termination of Membership:** Member’s may terminate Membership at any time upon 60 days advance written notice of termination and shall comply with the obligations in effect at the time of termination.
    2. A Non-Performing Member wishing to terminate membership must demonstrate their complete inability to perform obligations to an auditor assigned by the Service Provider.


## **Amendments**



1. Amendments to this Agreement require a majority in number of Members.
2. Amendments in conflict with the Aim and Principles are subject to veto by a majority in number of Guardians.
3. All Members enter into this agreement in good faith and hold harmless Members of the Economic Commons.


## **Entirety**

This agreement represents consent to the entirety of a mutual agreement between Members to the expressed common purpose and no other.


## **Notices**

Any notice given by the Members shall be valid only if delivered via the contact information for the Guardians. Notices include any votes to change the content of this agreement.


## **Official Signatories**

**In WITNESS WHEREOF**, the duly authorized Guardians of the Economic Commons sign this agreement on the dates indicated below, and agree to abide by the terms of this Agreement.



1. Member Class or Witness: (Guardian, General Member, Core Service Provider)
2. Full Name:
3. Contact Information or Service: (e.g. email or phone number)
4. Proof of Identity: (e.g. Passport number and country or other proof)
5. Date of Signing:
6. Place of Signing:
7. Signature or Hash: