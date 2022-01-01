# Roadmap

## Custodial Systems

1. Objective: Launch CIC-Stack (v2 codebase) (MVP Launch Milestone in GL) {Q4_2021}

    1. Key Result: CIC-Stack contracts deployed to bloxberg mainnet
    1. Key Result: 100% of users migrated from Sempo/xDAI
    1. Key Result: Run 1 disaster recovery exercise and report findings and create DR playbook
    1. Key Result: Integration tests are ran on all commits to master
    1. Key Result: Able to output reports / dashboard on CIC data

1. Objective: make the monorepo less of a chore to run {Q4_2021}
    1.  Key Result: services use mounted code and hot reload
    1.  Key Result: the root README.md gives new users enough info to get started

## Community Distributed Services

1. Objective: Local Blockchain Development
    1. Key Result: Specifications for all shared ledger features with consistency with CIC legal and tech framework {Q1_2022}
    1. Key Result: Tested Interoperability between CIC Chains (BloxBerg and new chains) {Q3_2022}
    1. Key Result: New Chain deployed on a local CIC network with 5+ nodes {Q4_2022}

1. Objective: Local Micro Services {Q4_2022}
    1. Key Result: Specifications for deployment strategies for local services {Q1_2022}
    1. Key Result: Running in one local area POC {Q2_2022}
    1. Key Result: Teaching service providers {Q4_2022}

1. Objective: Bring online and offline content to those underserved {Q2_2022}
    1. Key Result: Deploy a mesh network
    1. Key Result: Create a CIC for broadband services
    1. Key Result: Create a CIC for offline local content

1. Objective: User should be able to share local content {Q2_2022}
    1. Key Result: Launch incentives for storage of content
    1. Key Result: Launch incentives for content publishers

## Trust Networks

1. Objective: Service Provider can create impact claims about user data {Q2_2022}
    1. Key Result: Develop spec on impact claims regarding CICs
    1. Key Result: visualize claims about a CIC
    1. Key Result: We deploy and visualize claims about software development
    1. Key Result: We enable supporters to contribute toward claims

1. Objective: Sarafu (gift token) is fairly issued to users {Q2_2022}
    1. Key Result: Users are co-endorsed before they get Sarafu or Sarafu disbursements (also for gas).

1. Objective: Service Providers and Users have the ability to connect to other tokens on other chains (bridging)
    1. Key Result: Able to create a liquidity pool between Sarafu and Eth via partners

## Privacy

1. Objective: To give users control over their own data
    1. Key Result: Research zkp for transactions
    1. Key Result: Research zkp other parameters

1. Objective: Censor Resiliency
    1. Key Result: Define secure tech for communications, data storage

## Tooling

1. Objective: Users can interact with multiple tokens on USSD {Q4_2021}
    1. Key Result: Users on the Grassroots Economics mainnet deployment can hold multiple tokens
    1. Key Result: Users can hold 100 tokens without performance degradation
    1. Key Result: Interview/test 2 chamas on UX of token creation and usage and report findings

1. Objective: Users can support each other to unlock / recover pins {Q4_2021}
    1. Key Result: Launch a social recovery feature
    1. Key Result: 50% of new users using the social recovery function

1. Objective: Users can see and choose recent/common contacts/recipients {Q1_2022}
    1. Key Result: Users don't have to lookup common numbers

1. Objective: Users can discover and present goods and services in their community  (Directory) {Q1_2022}
    1. Key Result: API's are speced and deployed
    1. Key Result: a USSD interface created
    1. Key Result: Record 5 user stories on the new system and report create a report
    1. Key Result: 10% of active users have used the directory
    1. Key Result: deploy a web based marketplace
    1. Key Result: Interview 5 users and create a ux report

1. Objective: Create a web interface to CIC Stack (Custodial Web wallet) {Q1_2022}
    1. Key Result: API interfaces allow for feature parity with USSD interface (rest)
    1. Key Result: Create a CLI tool for testing
    1. Key Result: deploy a web based custodial web wallet
    1. Key Result: Interview 5 users for feedback and create a report

1. Objective: Users have the option for exchanging CIC's with one-time codes / scratch cards {Q1_2022}
    1. key result: print cards with onetime code

1. Objective: Users can interface with CICs and hold their own keys (Non-custodial wallet spec)
    1. Key Result: Specifications for all CIC features on a non-custodial wallet

1. Objective: Users can rate each others' goods and services and share those ratings on a marketplace / directory  {Q2_2022}
    1. Key Result: Rating menu item
    1. Key Result: Utilize ratings in Directory

1. Objective: Users can interface with CICs and hold their own keys (Non-custodial wallet)  {Q3_2022}
    1. Key Result: Able to provide all the same features on a non-custodial wallet - via a partner

1. Objective: Users can create their own CIC on the web {Q2_2022}
    1. Key Result: DAO CIC creation structure
    1. Key Result: Launch website

1. Objective: Empower users to vote on how community resources are used {Q2_2022}
    1. Key Result: Launch an interface for voting for redistribution of demurrage
    1. Key Result: Launch an interface for voting proposals

## Security

1. Objective: Create a foundational security audit of our core contracts and services
    1. Key Result: Static analysis is ran on all deployed contracts as part of automated testing
    1. Key Result: Audit our service deployment and create a report of security vulnerabilities
    1. Key Result: Create a quarterly report of our progress with the trail-of-bits security workflow https://github.com/crytic/building-secure-contracts/blob/master/development-guidelines/workflow.md

1. Objective: We want a comprehensive understanding of our attack surface
    1. Key Result: Static analysis is ran on all bridging contracts to other chains

1. Objective: Ensure we have enough gas security
    1. Key Result: Demonstrate that we have or can mine enough gas to be in operation for 2 years

## Contributor Experience

1. Objective: Our codebase has a great onboarding experience
    1. Key Result: Include a code of conduct for the Grassroots Economics is in the monorepo
    1. Key Result: The README describes how to build the monorepo and test
    1. Key Result: Documentation website
    1. Key Result: create a strategy for chat communications
    1. Key Result: Re-deploy Nextcloud for team
    1. Key Result: All pr's use a "fork and pr" flow. Create a tutorial on how to  do this.
    1. Key Result: Deploy a Discourse forum and use it for longform content like RFC's and operational changes
    1. Key Result: Design track growth of our project (how many new contributes to chat/code/contribute)
    1. Key Result: we a clear strategy around git self hosting and contributor experience
    1. Key Result: All of our in-house code dependencies have test, ci, semver tagging and publish to relevant registry (e.g, pypi etc)

## Legal

1. Objective: Clear legal framework for CIC issuance and service provision
    1. Key Result: A Clearing Union Charter {Q4_2021}
    1. Key Result: A Service Agreement contract for CIC creation and GE services {Q4_2021}
    1. Key Result: New round of Legal Due Diligence {Q1_2022}

## Implementations

1. Objective: Demonstrate CIC usage with marginalized communities
    1. Key Result: Implement a RCT showing the impact of CIC using a multitoken wallet
    1. Key Result: Develop modules for humanitarian organizations - Red Cross, WFP, GIZ, UNICEF, Mustard Seed
