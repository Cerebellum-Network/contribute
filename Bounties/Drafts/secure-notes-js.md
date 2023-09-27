# Secure Note Sharing Application Demo on DDC
Demonstrate the power and security of Cere DDC cloud storage platform by launching a Note sharing application with [Cere DDC-SDK-JS](https://github.com/CereNetwork/ddc-sdk-js) and earn $250 per milestone completed!

## Background
Developers and the general public often need to share code, notes and other text-only snippets. There are many applications on the web that enable this, including [Github Gists](https://gist.github.com), [Pastebin](https://pastebin.com/) and [Privnote](https://privnote.com/). At their core, each are simple, yet powerful and widely used services for sending notes to anyone on the web. 

For inspiration or a base from which to start building your note sharing application, we believe these repo's and tutorial resources might be helpful: 

- Pastebin: [@JoeBiellik/paste](https://github.com/JoeBiellik/paste), [@mstallmo/paste.rs](https://github.com/mstallmo/paste.rs)
- Privnote: [How to Build a Privnote Clone](https://remarkablemark.org/blog/2022/04/23/how-to-build-a-privnote-clone/), [@remarkablemark/Replit-Privnote](https://github.com/remarkablemark/Replit-Privnote)

By integrating your note sharing application with Cere's **[DDC-SDK-JS](https://github.com/CereNetwork/ddc-sdk-js)**, we aim to bring the benefits of decentralized cloud storage to this secure note-sharing platform. The Cere DDC SDK is a software development kit for interacting with Cere's Decentralized Data Cloud that empowers developers to build secure applications powered by the Decentralized Data Cloud. Some of the features you might use to complete this project are:

- [Content Addressable Storage](https://github.com/Cerebellum-Network/cere-ddc-sdk-js/blob/main/packages/content-addressable-storage/README.md)
- [Key Value Storage](https://github.com/Cerebellum-Network/cere-ddc-sdk-js/blob/main/packages/key-value-storage/README.md)
- [Data Encryption](https://github.com/Cerebellum-Network/cere-ddc-sdk-js/blob/main/packages/core/README.md#cipher)
- [DDC Client](https://github.com/Cerebellum-Network/cere-ddc-sdk-js/blob/main/packages/ddc-client/README.md)


## Deliverables
### Milestone 1 - Public Notes
* Estimated duration: 1 day

1. Locally deployable Note sharing application.
 - New Bucket is created and funded with [Cere Testnet](https://stats.cere.network/faucet) tokens.
2. End-User should be able to complete the following tasks using a simple Javascript based web-ui:
 - Create and save a new PUBLIC (unencrypted) "note"++ to the application specific bucket.
 - Load and view the previously created PUBLIC "note".
 - Delete existing PUBLIC "note" (or otherwise make the "note" inaccessible).
3. Basic error handling (404: not found).
4. A clear README with deployment and feature descriptions.

++ Notes should have a maximum upload size of 1MB.

### Milestone 2 - Private + Secure Notes
* Estimated duration: 1 day

5. End-User should be able to complete the following tasks:
- Create and save a new PRIVATE (unencrypted) "note" that can only be opened ONE-TIME or 2) expires after set time-limit.
- Load and be able to view an un-expired PRIVATE "note" ONE-TIME.
- Create and save a new SECURE (encrypted) "note", which only a specified wallet address owner can read.
- Load and view the existing SECURE "note" from specified wallet address. 
7. Additional error handling (401: not authorized).

### Not in Scope
* It is not necessary for the application to have any additional features or design elements other than those necessary to complete the required deliverables.

## Resources
* To learn more about how to build applications with the latest version of Cere DDC JS, see the [Cere Developer Quickstart Guidebook](https://docs.cere.network/ddc/developer-guide/quickstart).

## About the Team
- Your Name (ROLE @ ORG): Bio (in third-person), with links to socials

## Additional Information

*Add any additional information about your solution to this bounty that hasn't already been included.*






--- 

## How to Apply
Interested? Apply following these steps:
1. Clone [this repository](https://github.com/Cerebellum-Network/contribute).
2. Create a new branch.
3. Fill in the remaining details of *this* pre-prepared bounty proposal (ie, the file you are reading now).
4. Move to `../Active` folder and commit and push the changes to your forked version of the repository.
5. [Submit a PR](https://github.com/Cerebellum-Network/contribute/pulls) against Cerebellum's upstream main branch for approval.

## Approval Workflow
1. Initial Review: The Cere Contributor team will provide initial feedback within 3 business days of PR submission.
2. Feedback Loop: Necessary revisions will be communicated in the respective Github PR until a winner is chosen.
3. Approval and Payout: Upon approval and merging of the PR + KYC, the bounty will be distributed to the winner, per negotiated terms.

## Terms and Conditions
1. Eligibility: Open to individuals 18 years and older. Only 1 winner will be approved for this bounty.
2. Ownership: All submitted code must be original or otherwise attributed according to license requirements.
3. Licensing: Code must be open-sourced and compatible with the original repository.
4. Disqualification: Failure to meet requirements or deadlines leads to disqualification.
5. Liability: Organizers are not liable for any issues arising from the bounty.
6. Amendments: Organizers may change the terms and conditions at any time. Version history can be tracked in Github commit logs.
7. Do your own research. Do not share sensitive data or deploy to production without proper testing, code audits, etc.

---
🛟 Questions? Ask in our [Contributor Discord](https://cere.network/discord) or write us at [community@cere.io](mailto:community@cere.io).
