# Cere Bug Bounty
Cere invites bug hunters, security experts and ethical hackers to identify and report potential bugs and security vulnerabilities in the Cere Network ecosystem. We believe that by taking a proactive approach we improve the network’s security, ensuring a safer environment for all current and future users and their data. 

## Background
Cere is a decentralized blockchain and p2p cloud storage protocol built for handling all classes of cross-chain storage workloads, enabling projects to keep their data safe, in a decentralized, permissionless and interoperable environment based on Substrate and our own decentralized data protocol the Decentralized Data Cloud or DDC. 

With Cere Network and the DDC being such a complex system, plus the fact there are real-value digital assets at stake, it’s critical that additional resources are allocated to ensuring the core code commits in the ecosystem should get as many reviews as possible, to minimize risk of exposure to bugs and other issues that might result in system malfunction and loss of funds or data.

## How to Start
- Step 1: Sign-up via [this form](https://noteforms.com/forms/contributor-sign-up) to register as a Contributor.
- Step 2: Report any potential issues discovered.
  ⚠️ **DO NOT CREATE ANY PUBLIC ISSUE OR POSTS related to (potential) security related findings**. See the [Responsible Disclosure](https://www.notion.so/Cere-Bug-Bounty-d6d2b20f473d43d39c93294335e29015?pvs=21) section below for more details.

That’s it! A member of the the Cere Community team will reach out about your experience completing this mission and clarify any final questions regarding your registration and share additional details about getting started onboarding to Cere Network.

## Bounty Payouts
Cere Bounty payouts for issues reported are as follows:
💡 Legend - Severity Levels & Payouts
- Critical   |  $5,000 - $10,000+
- High       |  $1,000 - $5,000
- Medium     |  $500 - $1,000
- Low & Info |  $50 - $500
🔏 All reports will be assessed by independent security auditors for final severity rating.

## Payment
- The CERE/USD conversion rate used for payments is the average market price for the month in which the bug was submitted.
- The reference for this price is calculated based on the Closing Price given by Coingecko.com given [here](https://www.coingecko.com/en/coins/cere-network).
- The final severity and payout recommendation of all valid issues reported are decided by the Cere Bug Bounty Team, with consultation with Halborn security team and other third-party security consultants, if necessary. We will make this as transparent of a process as possible to ensure all parties are satisfied and agree with the outcome.

## In Scope
These vulnerabilities often require a deep understanding of both traditional web security and the unique aspects of blockchain technology. Each of these topics has its own set of challenges and requires specialized knowledge to tackle effectively.
- **Smart Contract Vulnerabilities**: This is often the most critical area in Web3 bug bounties. Issues can range from reentrancy attacks, integer overflows, and unauthorized access to funds or data. Understanding the Solidity programming language and the Ethereum Virtual Machine (EVM) is crucial for identifying these vulnerabilities.
- **Decentralized Finance (DeFi) Exploits**: With the rise of DeFi platforms, vulnerabilities in lending protocols, yield farming contracts, and decentralized exchanges (DEXs) have become increasingly common. Bugs in these areas can lead to massive financial losses.
- **Front-End Security**: Even though the blockchain backend might be secure, vulnerabilities in the front-end can expose users to risks like phishing attacks, wallet manipulations, and data leaks. Ensuring the security of Web3-enabled browsers and extensions like MetaMask is essential.
- **Oracles and Data Feeds**: Oracles provide external data to smart contracts and are a common point of failure. Manipulating oracles can lead to incorrect data being fed into smart contracts, causing unintended behavior.> 
- **Governance and Voting Mechanisms**: Many Web3 platforms have governance tokens and voting systems to make collective decisions. Vulnerabilities in these systems can lead to unfair voting, token minting, or changes in critical platform parameters.
- **Front-End Vulnerabilities**: As mentioned earlier, issues like Cross-Site Scripting (XSS) and Cross-Site Request Forgery (CSRF) can be particularly damaging in a Web3 context, where users often interact with decentralized applications through web interfaces.
- **Phishing Attacks**: Given the irreversible nature of blockchain transactions, phishing attacks that trick users into revealing their private keys or sending funds to malicious addresses are a significant concern.
- **Sybil Attacks**: In decentralized networks, Sybil attacks involve creating multiple fake identities to subvert the functioning of the network. This can be particularly problematic in peer-to-peer networks and decentralized identity systems.
- **Node Vulnerabilities**: Full nodes, mining nodes, and other network participants can have vulnerabilities that allow attackers to crash the network or perform other malicious activities.
- **Replay Attacks**: In some cases, transactions on one blockchain can be replayed on another blockchain, leading to unintended financial consequences. This is often a concern during blockchain forks.
- **Eclipse Attacks**: In this type of attack, an attacker monopolizes all of the victim's incoming and outgoing connections, effectively isolating the victim from the rest of the network.
- **Routing Attacks**: Given that many blockchain networks operate over peer-to-peer protocols, they are susceptible to routing attacks like BGP hijacking, which can redirect network traffic through malicious nodes.
- **Data Exposure**: Improperly secured IPFS nodes or other decentralized storage solutions can expose sensitive user data.
- **Authorization Flaws**: Incorrect implementation of roles and permissions can lead to unauthorized actions, especially in multi-signature or governance contracts.
- **Timestamp Manipulation**: Some smart contracts rely on block timestamps for functionality. Manipulating these can lead to unintended contract behavior.
- **Denial of Service (DoS)**: Overloading network nodes or smart contracts by exploiting gas costs can make the system unresponsive.
    
## Cere Projects
### Smart Contracts
- DDC: https://github.com/Cerebellum-Network/ddc-bucket-contract
- Freeport: https://github.com/Cerebellum-Network/Freeport-Smart-Contracts

### SDKs
- Cere Games SDK: [https://github.com/cere-io/cere-games-sdk](https://github.com/cere-io/cere-games-sdk/issues)
- DDC SDK JS: https://github.com/Cerebellum-Network/cere-ddc-sdk-js
- DDC SDK Go: https://github.com/Cerebellum-Network/cere-ddc-sdk-go
- DDC SDK Kotlin: https://github.com/Cerebellum-Network/cere-ddc-sdk-kotlin
- Freeport Smart Contracts SDK: https://github.com/Cerebellum-Network/Freeport-Smart-Contracts-SDK
- Freeport NFT Marketplace Client: https://github.com/cere-io/nft-marketplace-client

### Blockchain Tools & Services
- Blockchain Substrate Bridge (Stage): https://bridge.stage.cere.network/
 - https://github.com/Cerebellum-Network/chainbridge-ui
 - https://github.com/ChainSafe/chainbridge-core
- Blockchain Explorer (Stage): https://explorer.stg.cere.network/
 - https://github.com/Cerebellum-Network/explorer
 - Blockchain Staking Dashboard (Stage): https://staking-stg.network-stage.aws.cere.io/#/overview
- Blockchain Staking Dashboar (Stage)
 - https://github.com/Cerebellum-Network/staking-dashboard
- Blockchain Stats (Stage): https://stats.stg.cere.network/
 - https://github.com/Cerebellum-Network/cerestats
    
### Front-ends
 - Freeport Website (Stage): [https://freeport.stg.cere.network](https://freeport.stg.cere.network/)
 - CerePlay Game Portal Website (Stage): [https://games.stg.cere.network](https://games.stg.cere.network/)
 - Cere Wallet Website (Stage): [https://wallet.stg.cere.io](https://wallet.stg.cere.io/)

## Out of Scope
- Production [Cere.network](http://Cere.network) & [Cere.io](https://www.notion.so/fbc441b4e8ba42b0bd44c62ebc5220cd?pvs=21) websites, Cere infrastructure and all Cere Mainnet protocol’s, dApps, and related tools & utilities are outside the scope of this program.
- Smart contracts deployed on the Cere Network Blockchain or DDC Mainnet are not a part of the bug bounty program.
- Bugs from third-party tools we use, such as Discord, Telegram, WordPress, etc., should be reported to those services directly. Bugs from these third parties will not qualify for this program.
- Also out of scope are the *third-party services and websites* integrating with Cere Network.

⚠️ The following activities are specifically prohibited by this bug bounty program:
- Any testing with Cere Mainnet contracts.
- Any testing with pricing oracles or third party smart contracts
- Attempting phishing or other social engineering attacks against our employees and/or customers
- Any testing with third party systems and applications (e.g. browser extensions) as well as websites (e.g. SSO providers, advertising networks)
- Any denial of service attacks
- Automated testing of services that generates significant amounts of traffic
- Public disclosure of an unpatched vulnerability in an embargoed bounty

# Issue Reporting Guidelines
All bug reports must come with a clear example, and clear steps to reproduce in order to be considered for a reward.

We strongly recommend video recording all testing sessions! Provide relevant screenshots, docs, and code necessary to reproduce the issue.

Check [this page](https://www.notion.so/fa040a9d146b46969622fbf2aa493fc6?pvs=21) for an example of a good bug report.

### Security Vulnerabilities
To be eligible for a reward related to *high impact or security related issues* which could negatively impact the execution of the Blockchain Network or DDC or expose customer data or funds to risk if exploited, etc must be reported privately! 

⚠️ **DO NOT CREATE ANY PUBLIC ISSUE OR POSTS related to (potential) security related findings**. 

Instead, send an email to security@cere.io, sharing your preferred contact method (email, telegram, discord, etc) along with your github handle. We will get back to you within 1 business day with confirmation of receiving your report and proposed next steps. [Learn more](https://www.notion.so/Responsible-Disclosure-Policy-ced2b2c1238f403e9f44b692f6e2c695?pvs=21).

Responsible disclosure includes adhering to strict confidentiality and not publishing sensitive information in public, on Github, or anywhere else that might compromise this program’s operational security. 

If you’re not sure, reach out via [security@cere.io](https://www.notion.so/b9db00101824422f8a7c29de5e7c9c7a?pvs=21) with any questions.

### General Issues & Other Feedback
For general feedback, share your discoveries using this form  ⇒ https://cere.network/feedback.

All other issues and feature requests should be submitted to Github:
- https://github.com/orgs/Cerebellum-Network
- https://github.com/cere-io

## Eligibility
Additionally, you are **eligible** to participate in the Program if you meet **all** of the following criteria:
- You are of legal age and have the legal capacity to give your consent to the terms of these Program Rules.
- You have followed the [responsible disclosure policy](https://www.notion.so/Responsible-Disclosure-Policy-ced2b2c1238f403e9f44b692f6e2c695?pvs=21).
    
Responsible disclosure includes adhering to strict confidentiality and not publishing sensitive information in public, on Github, or anywhere else that might compromise this program’s operational security. 
- You are able to send an invoice for the payment, unless otherwise negotiated.
- If you are acting in the name of and on behalf of your employer, you must clearly state this during the Registration Process and confirm that you are authorized to give your consent to the terms of these Program Rules in the name of and on behalf of your employer. You are responsible for reviewing your employer's rules for participating in this Program. Cere disclaims any and all liability or responsibility for disputes arising between you and your employer related to this matter.
- Public Sector Employee: if you are a public sector employee, please contact our Bug Bounty team at [security@cere.io](mailto:security@cere.io) using the details above prior to any testing activities

You are **not eligible** to participate in the Program if you meet **any** of the following criteria:
- You do not fulfill all the above criteria
- You are a resident or a national of any country subject to international or Swiss sanctions
- You are a resident or a national of any country that does not allow participation in this type of Program
- You are currently an employee of Cere, or an immediate family or household member of such an employee
- Within the six months prior to providing us your Submission, you were an employee of Cere
- You currently (or within six months prior to providing us your Submission) perform services for Cere or a Cere subsidiary in an external staff capacity that requires access to the Cere Network, such as agency temporary worker, vendor employee, contractor.

## Contact Us
For general inquiries, write us with any questions at [community@cere.io](https://www.notion.so/Cere-Bug-Bounty-d6d2b20f473d43d39c93294335e29015?pvs=21).

To report a potential security issue, write us at [security@cere.io](mailto:security@cere.io). 
Learn more about our [Responsible Disclosure Policy](https://www.notion.so/Responsible-Disclosure-Policy-ced2b2c1238f403e9f44b692f6e2c695?pvs=21).

# Appendix
## Severity Legend
- **Critical**: Critical severity issues present a direct and immediate risk to a broad array of our users or to a Cere network product itself. 
**High**: High severity issues allow an attacker to read or modify highly sensitive data that they are not authorized to access. They are generally more narrow in scope than critical issues, though they may still grant an attacker extensive access.
- **Medium**: Medium severity issues allow an attacker to read or modify limited amounts of data that they are not authorized to access. They generally grant access to less sensitive information than high severity issues.
- **Low & Info**: Low & informational issues allow an attacker to access extremely limited amounts of data. They may violate an expectation for how something is intended to work but allow nearly no escalation of privilege or ability to trigger unintended behavior by an attacker.

