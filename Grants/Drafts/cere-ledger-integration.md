# CERE Ledger Integration - Grant up to $25,000+
Cere invites proposals from qualified external developers to deliver Ledger hardware support for Cere Network, a Substrate based nPoS blockchain.

## Grant Objective
The Cere Community has frequently expressed the need for hardware wallet compatibility. Ledger, known for its Ledger Nano S and Ledger Nano X, stands out as a leading hardware wallet provider. This bounty serves as an open call for community proposals to integrate Cere Blockchain with Ledger Wallet.

## Background
To support Substrate-based networks like Cere Network on Ledger devices, the following features are generally needed:
1. **Network-Specific Ledger App**: A dedicated app for the Substrate-based network needs to be developed for Ledger devices.
2. **Third-Party Wallet Integration**: Even if Ledger Live doesn't support the network, the Ledger device should be compatible with a third-party wallet that does.
3. **Transaction Signing**: Ledger devices should support the network's unique transaction formats for signing and verification.
4. **Asset Management**: The Ledger device must support the storage and management of native tokens and other assets on the network.
5. **Firmware Updates**: The device should be capable of firmware updates to incorporate future changes in the network's protocol.
6. **Secure Communication**: Proper encryption and secure communication channels must be in place between the Ledger device and the network.

The active development community around a specific Substrate-based network can expedite its Ledger support by focusing on these features.

### **Reference Materials**
- **[Guidelines for App Publishing — Ledger Documentation Hub](https://ledger.readthedocs.io/en/latest/additional/publishing_an_app.html)**
- Monero BOLOS App: **[GitHub Repository](https://github.com/LedgerHQ/app-monero)**

## Deliverables
The scope of the project includes the development of a Cere application compatible with both Ledger Nano S and X, encompassing the following elements:
- BOLOS application for Ledger Nano S/X 
 - (**[Feature Details](#appendix) below for further details**)
- Technical Specifications and Documentation
- C++ Unit Testing
- Zemu Test Suites
All developed code should be hosted on GitHub and, upon project completion, transferred to the **[Cerebellum-Network GitHub organization](https://github.com/Cerebellum-Network)** under an Apache 2.0 License.

## Reward
Your project could receive up to $25,000 along with additional free cloud storage.

## Evaluation Criteria
1. Technical expertise in blockchain development, particularly on Substrate.
2. Previous experience in developing staking or DeFi solutions.
3. Budget and timeline feasibility.
4. Quality and innovation of the proposed solution.

## Submission Guidelines
Only one submission will be approved per person/team/project/request.
The project proposal with the most promise will be selected for completion.

## Attribution and Social Media
The final project will be featured on the **[Cere Network Blog](https://cere.network/blog)**, with your name credited as the contributing developer. We can also reference your Twitter handle in our public posts about the project.

### How to Apply
Simple! Here are the step’s you should take to get the application process started:
1. Tweet publicly a short description @CereOfficial of your idea for how you’ll use Cere DDC for decentralized storage in a few sentences. If our main account retweets your tweet, well, that’s step 1 complete!
2. Join and share your tweet with our incredible [Contributor Discord](http://cere.network/discord) community as well. Ask for feedback and suggestions how to improve.
3. Prepare your project proposal draft
 - **Project Name**: A name that uniquely identifies your project.
 - **Project Description**: A detailed description of what you're buildind, how you plan to use DDC and why you (or your team) is interested.
 - **Team Details:** Include a brief overview of your (and the rest of your team’s) background, and expected project roles and responsibilities.
 - **Project Roadmap:** A brief description of what has been done already (directly or indirectly), and a summary of project milestones and deliverables, with estimated time and cost expected to complete each milestone, or any other resources required.
4. Submit your application using this [form](https://noteforms.com/forms/cere-bounties-submission-zivk7s).

That’s it! A member of the the Cere Community team will reach out about your experience completing this mission and clarify any final questions regarding the bounty reward distribution, etc within 24-72h.

### Community Engagement: How to Gather Support
To garner community support, announce your project on Twitter and in the **[Cere Contributor Discord](https://cere.network/discord)**. Share updates and seek feedback. Additionally, we're offering free public and private cloud storage buckets for mutable and immutable data sets that can be streamed, are content-addressable, and more. This is a unique feature that can attract more community interest in your project.
By actively engaging with the community, you can gather valuable feedback and support for your project. This is your chance to contribute to the future of decentralized cloud storage in IoT, so seize it!

# Appendix
## Feature Support
- System
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Remark |  | ✅ | ✅ | ✅ | Bytesremark |
    | Set heap pages |  | ✅ | ✅ | ✅ | u64pages |
    | Set code |  | ✅ | ✅ | ✅ | Vecu8code |
    | Set code without checks |  | ✅ | ✅ | ✅ | Vecu8code |
    | Set storage |  |  |  |  | VecKeyValueitems |
    | Kill storage |  |  |  |  | VecKeykeys |
    | Kill prefix |  |  |  |  | Keyprefixu32subkeys |
    | Remark with event |  | ✅ | ✅ | ✅ | Bytesremark |

- Scheduler
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Schedule |  |  |  |  | BlockNumberwhenOptionschedulePeriodBlockNumbermaybe_periodicschedulePrioritypriorityCallcall |
    | Cancel |  |  |  |  | BlockNumberwhenu32index |
    | Schedule named |  |  |  |  | TaskNameidBlockNumberwhenOptionschedulePeriodBlockNumbermaybe_periodicschedulePrioritypriorityCallcall |
    | Cancel named |  |  |  |  | TaskNameid |
    | Schedule after |  |  |  |  | BlockNumberafterOptionschedulePeriodBlockNumbermaybe_periodicschedulePrioritypriorityCallcall |
    | Schedule named after |  |  |  |  | TaskNameidBlockNumberafterOptionschedulePeriodBlockNumbermaybe_periodicschedulePrioritypriorityCallcall |

- Babe
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Report equivocation |  |  |  |  | BoxEquivocationProofHeaderequivocation_proofKeyOwnerProofkey_owner_proof |
    | Report equivocation unsigned |  |  |  |  | BoxEquivocationProofHeaderequivocation_proofKeyOwnerProofkey_owner_proof |
    | Plan config change |  |  |  |  | NextConfigDescriptorconfig |

- Timestamp
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Set |  | ✅ | ✅ |  | Compactu64now |

- Indices
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Claim |  | ✅ | ✅ |  | AccountIndexindex |
    | Transfer |  | ✅ | ✅ |  | AccountIdLookupOfTnew_AccountIndexindex |
    | Free |  | ✅ | ✅ |  | AccountIndexindex |
    | Force transfer |  | ✅ | ✅ |  | AccountIdLookupOfTnew_AccountIndexindexboolfreeze |
    | Freeze |  | ✅ | ✅ |  | AccountIndexindex |

- Balances
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Transfer | ✅ | ✅ | ✅ | ✅ | AccountIdLookupOfTdestCompactBalanceamount |
    | Set balance |  | ✅ | ✅ | ✅ | AccountIdLookupOfTwhoCompactBalancenew_freeCompactBalancenew_reserved |
    | Force transfer | ✅ | ✅ | ✅ | ✅ | AccountIdLookupOfTsourceAccountIdLookupOfTdestCompactBalanceamount |
    | Transfer keep alive | ✅ | ✅ | ✅ | ✅ | AccountIdLookupOfTdestCompactBalanceamount |
    | Transfer all | ✅ | ✅ | ✅ |  | AccountIdLookupOfTdestboolkeep_alive |
    | Force unreserve |  | ✅ | ✅ |  | AccountIdLookupOfTwhoBalanceamount |

- Authorship
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Set uncles |  |  |  |  | VecHeadernew_uncles |

- Staking
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Bond | ✅ | ✅ | ✅ | ✅ | AccountIdLookupOfTcontrollerCompactBalanceamountRewardDestinationpayee |
    | Bond extra | ✅ | ✅ | ✅ |  | CompactBalanceamount |
    | Unbond | ✅ | ✅ | ✅ | ✅ | CompactBalanceamount |
    | Withdraw Unbonded | ✅ | ✅ | ✅ |  | u32num_slashing_spans |
    | Validate | ✅ | ✅ | ✅ |  | ValidatorPrefsprefs |
    | Nominate | ✅ | ✅ | ✅ | ✅ | VecAccountIdLookupOfTtargets |
    | Chill | ✅ | ✅ | ✅ | ✅ |  |
    | Set payee | ✅ | ✅ | ✅ |  | RewardDestinationpayee |
    | Set controller | ✅ | ✅ | ✅ | ✅ | AccountIdLookupOfTcontroller |
    | Set validator count |  | ✅ | ✅ |  | Compactu32new_ |
    | Increase validator count |  | ✅ | ✅ |  | Compactu32additional |
    | Scale validator count |  | ✅ | ✅ |  | Percentfactor |
    | Force no eras |  | ✅ | ✅ |  |  |
    | Force new era |  | ✅ | ✅ |  |  |
    | Set invulnerables |  | ✅ | ✅ |  | VecAccountIdinvulnerables |
    | Force unstake |  | ✅ | ✅ |  | AccountIdstashu32num_slashing_spans |
    | Force new era always |  | ✅ | ✅ |  |  |
    | Cancel deferred slash |  | ✅ | ✅ |  | EraIndexeraVecu32slash_indices |
    | Payout stakers | ✅ | ✅ | ✅ |  | AccountIdvalidator_stashEraIndexera |
    | Rebond | ✅ | ✅ | ✅ |  | CompactBalanceamount |
    | Reap stash |  | ✅ | ✅ |  | AccountIdstashu32num_slashing_spans |
    | Kick |  | ✅ | ✅ |  | VecAccountIdLookupOfTwho |
    | Set staking configs |  | ✅ | ✅ |  | ConfigOpBalanceOfTmin_nominator_bond, ConfigOpBalanceOfTmin_validator_bond, ConfigOpu32max_nominator_count, ConfigOpu32max_validator_count, ConfigOpPercentchill_threshold, ConfigOpPerbillmin_commission |
    | Chill other |  | ✅ | ✅ |  | AccountIdcontroller |
    | Force apply min commission |  | ✅ | ✅ |  | AccountIdvalidator_stash |
    | Set min commission |  | ✅ | ✅ |  | Perbillnew_ |

- Session
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Set keys | ✅ | ✅ | ✅ |  | KeyskeysBytesproof |
    | Purge keys | ✅ | ✅ | ✅ |  |  |

- Grandpa
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Report equivocation |  |  |  |  | BoxEquivocationProofHashBlockNumberequivocation_proofKeyOwnerProofkey_owner_proof |
    | Report equivocation unsigned |  |  |  |  | BoxEquivocationProofHashBlockNumberequivocation_proofKeyOwnerProofkey_owner_proof |
    | Note stalled |  |  |  |  | BlockNumberdelayBlockNumberbest_finalized_block_number |

- ImOnline
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Heartbeat |  |  |  |  | HeartbeatBlockNumberheartbeatAuthorityIdasRuntimeAppPublicSignaturesignature |

- Democracy
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Propose |  | ✅ | ✅ | ✅ | BoundedCallOfTproposalCompactBalanceamount |
    | Second |  | ✅ | ✅ | ✅ | Compactu32proposal |
    | Vote |  | ✅ | ✅ | ✅ | Compactu32ref_indexAccountVotevote |
    | Emergency cancel |  | ✅ | ✅ | ✅ | ReferendumIndexref_index |
    | External propose |  | ✅ | ✅ | ✅ | BoundedCallOfTproposal |
    | External propose majority |  | ✅ | ✅ | ✅ | BoundedCallOfTproposal |
    | External propose default |  | ✅ | ✅ | ✅ | BoundedCallOfTproposal |
    | Fast track |  | ✅ | ✅ | ✅ | H256proposal_hashBlockNumbervoting_periodBlockNumberdelay |
    | Veto external |  | ✅ | ✅ | ✅ | H256proposal_hash |
    | Cancel referendum |  | ✅ | ✅ | ✅ | Compactu32ref_index |
    | Delegate |  | ✅ | ✅ | ✅ | AccountIdLookupOfTtoConvictionconvictionBalancebalance |
    | Undelegate |  | ✅ | ✅ | ✅ |  |
    | Clear public proposals |  | ✅ | ✅ | ✅ |  |
    | Unlock |  | ✅ | ✅ | ✅ | AccountIdLookupOfTtarget |
    | Remove vote |  | ✅ | ✅ | ✅ | ReferendumIndexindex |
    | Remove other vote |  | ✅ | ✅ | ✅ | AccountIdLookupOfTtargetReferendumIndexindex |
    | Blacklist |  | ✅ | ✅ |  | H256proposal_hashOptionReferendumIndexmaybe_ref_index |
    | Cancel proposal |  | ✅ | ✅ | ✅ | Compactu32prop_index |

- Council
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Set members |  | ✅ | ✅ |  | VecAccountIdnew_membersOptionAccountIdprimeMemberCountold_count |
    | Execute |  | ✅ | ✅ |  | ProposalproposalCompactu32length_bound |
    | Propose |  | ✅ | ✅ |  | Compactu32thresholdProposalproposalCompactu32length_bound |
    | Vote |  | ✅ | ✅ |  | HashproposalCompactu32indexboolapprove |
    | Close old weight |  | ✅ | ✅ |  | Hashproposal_hashCompactu32indexCompactu64proposal_weight_boundCompactu32length_bound |
    | Disapprove proposal |  | ✅ | ✅ |  | Hashproposal_hash |
    | Close |  | ✅ | ✅ |  | Hashproposal_hashCompactu32indexWeightproposal_weight_boundCompactu32length_bound |

- TechnicalCommittee
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Set members |  | ✅ | ✅ |  | VecAccountIdnew_membersOptionAccountIdprimeMemberCountold_count |
    | Execute |  | ✅ | ✅ |  | ProposalproposalCompactu32length_bound |
    | Propose |  | ✅ | ✅ |  | Compactu32thresholdProposalproposalCompactu32length_bound |
    | Vote |  | ✅ | ✅ |  | HashproposalCompactu32indexboolapprove |
    | Close old weight |  | ✅ | ✅ |  | Hashproposal_hashCompactu32indexCompactu64proposal_weight_boundCompactu32length_bound |
    | Disapprove proposal |  | ✅ | ✅ |  | Hashproposal_hash |
    | Close |  | ✅ | ✅ |  | Hashproposal_hashCompactu32indexWeightproposal_weight_boundCompactu32length_bound |

- TechnicalMembership
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Add member |  | ✅ | ✅ |  | AccountIdLookupOfTwho |
    | Remove member |  | ✅ | ✅ |  | AccountIdLookupOfTwho |
    | Swap member |  | ✅ | ✅ |  | AccountIdLookupOfTremoveAccountIdLookupOfTadd |
    | Reset members |  | ✅ | ✅ |  | VecAccountIdmembers |
    | Change key |  | ✅ | ✅ |  | AccountIdLookupOfTnew_ |
    | Set prime |  | ✅ | ✅ |  | AccountIdLookupOfTwho |
    | Clear prime |  | ✅ | ✅ |  |  |

- Treasury
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Propose spend |  | ✅ | ✅ |  | CompactBalanceamountAccountIdLookupOfTbeneficiary |
    | Reject proposal |  | ✅ | ✅ |  | Compactu32proposal_id |
    | Approve proposal |  | ✅ | ✅ |  | Compactu32proposal_id |
    | Spend |  | ✅ | ✅ |  | CompactBalanceamountAccountIdLookupOfTbeneficiary |
    | Remove approval |  | ✅ | ✅ |  | Compactu32proposal_id |

- Vesting
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Vest |  | ✅ | ✅ |  |  |
    | Vest other |  | ✅ | ✅ |  | AccountIdLookupOfTtarget |
    | Vested transfer |  | ✅ | ✅ |  | AccountIdLookupOfTtargetVestingInfoschedule |
    | Force vested transfer |  | ✅ | ✅ |  | AccountIdLookupOfTsourceAccountIdLookupOfTtargetVestingInfoschedule |
    | Merge schedules |  | ✅ | ✅ |  | u32schedule1_indexu32schedule2_index |

- Utility
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Batch | ✅ | ✅ | ✅ |  | VecCallcalls |
    | As derivative |  | ✅ | ✅ |  | u16indexCallcall |
    | Batch all | ✅ | ✅ | ✅ |  | VecCallcalls |
    | Dispatch as |  |  |  |  | BoxPalletsOriginas_originCallcall |
    | Force batch | ✅ | ✅ | ✅ |  | VecCallcalls |
    | With weight |  | ✅ | ✅ |  | CallcallWeightweight |

- Identity
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Add registrar |  | ✅ | ✅ |  | AccountIdLookupOfTaccount |
    | Set identity |  | ✅ | ✅ |  | IdentityInfoinfo |
    | Set subs |  | ✅ | ✅ |  | VecTupleAccountIdDatasubs |
    | Clear identity |  | ✅ | ✅ |  |  |
    | Request judgement |  | ✅ | ✅ |  | Compactu32reg_indexCompactu128max_fee |
    | Cancel request |  | ✅ | ✅ |  | RegistrarIndexreg_index |
    | Set fee |  | ✅ | ✅ |  | Compactu32indexCompactu128fee |
    | Set account id |  | ✅ | ✅ |  | Compactu32indexAccountIdLookupOfTnew_ |
    | Set fields |  |  |  |  | Compactu32indexIdentityFieldsfields |
    | Provide judgement |  | ✅ | ✅ |  | Compactu32reg_indexAccountIdLookupOfTtargetJudgementBalanceOfTjudgementHashidentity |
    | Kill identity |  | ✅ | ✅ |  | AccountIdLookupOfTtarget |
    | Add sub |  | ✅ | ✅ |  | AccountIdLookupOfTsubDatadata |
    | Rename sub |  | ✅ | ✅ |  | AccountIdLookupOfTsubDatadata |
    | Remove sub |  | ✅ | ✅ |  | AccountIdLookupOfTsub |
    | Quit sub |  | ✅ | ✅ |  |  |

- Proxy
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Proxy |  | ✅ | ✅ | ✅ | AccountIdLookupOfTrealOptionProxyTypeforce_proxy_typeCallcall |
    | Add proxy |  | ✅ | ✅ |  | AccountIdLookupOfTdelegateProxyTypeproxy_typeBlockNumberdelay |
    | Remove proxy |  | ✅ | ✅ |  | AccountIdLookupOfTdelegateProxyTypeproxy_typeBlockNumberdelay |
    | Remove proxies |  | ✅ | ✅ |  |  |
    | Create pure |  | ✅ | ✅ |  | ProxyTypeproxy_typeBlockNumberdelayu16index |
    | Kill pure |  | ✅ | ✅ |  | AccountIdLookupOfTspawnerProxyTypeproxy_typeu16indexCompactu32heightCompactu32ext_index |
    | Announce |  |  |  |  | AccountIdLookupOfTrealCallHashOfcall_hash |
    | Remove announcement |  |  |  |  | AccountIdLookupOfTrealCallHashOfcall_hash |
    | Reject announcement |  |  |  |  | AccountIdLookupOfTdelegateCallHashOfcall_hash |
    | Proxy announced |  | ✅ | ✅ |  | AccountIdLookupOfTdelegateAccountIdLookupOfTrealOptionProxyTypeforce_proxy_typeCallcall |

- Multisig
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | As multi threshold 1 |  | ✅ | ✅ | ✅ | VecAccountIdother_signatoriesCallcall |
    | As multi |  | ✅ | ✅ | ✅ | u16thresholdVecAccountIdother_signatoriesOptionTimepointmaybe_timepointCallcallWeightmax_weight |
    | Approve as multi |  | ✅ | ✅ | ✅ | u16thresholdVecAccountIdother_signatoriesOptionTimepointmaybe_timepointH256call_hashWeightmax_weight |
    | Cancel as multi |  | ✅ | ✅ | ✅ | u16thresholdVecAccountIdother_signatoriesTimepointtimepointH256call_hash |

- Bounties
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Propose bounty |  | ✅ | ✅ |  | CompactBalanceamountBytesdescription |
    | Approve bounty |  | ✅ | ✅ |  | Compactu32bounty_id |
    | Propose curator |  | ✅ | ✅ |  | Compactu32bounty_idAccountIdLookupOfTcuratorCompactBalancefee |
    | Unassign curator |  | ✅ | ✅ |  | Compactu32bounty_id |
    | Accept curator |  | ✅ | ✅ |  | Compactu32bounty_id |
    | Award bounty |  | ✅ | ✅ |  | Compactu32bounty_idAccountIdLookupOfTbeneficiary |
    | Claim bounty |  | ✅ | ✅ |  | Compactu32bounty_id |
    | Close bounty |  | ✅ | ✅ |  | Compactu32bounty_id |
    | Extend bounty expiry |  | ✅ | ✅ |  | Compactu32bounty_idBytesremark |

- ChildBounties
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Add child bounty |  | ✅ | ✅ |  | Compactu32parent_bounty_idCompactBalanceamountVecu8description |
    | Propose curator |  | ✅ | ✅ |  | Compactu32parent_bounty_idCompactu32child_bounty_idAccountIdLookupOfTcuratorCompactBalancefee |
    | Accept curator |  | ✅ | ✅ |  | Compactu32parent_bounty_idCompactu32child_bounty_id |
    | Unassign curator |  | ✅ | ✅ |  | Compactu32parent_bounty_idCompactu32child_bounty_id |
    | Award child bounty |  | ✅ | ✅ |  | Compactu32parent_bounty_idCompactu32child_bounty_idAccountIdLookupOfTbeneficiary |
    | Claim child bounty |  | ✅ | ✅ |  | Compactu32parent_bounty_idCompactu32child_bounty_id |
    | Close child bounty |  | ✅ | ✅ |  | Compactu32parent_bounty_idCompactu32child_bounty_id |

- Tips
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Report awesome |  | ✅ | ✅ |  | BytesreasonAccountIdLookupOfTwho |
    | Retract tip |  | ✅ | ✅ |  | Hashhash |
    | Tip new |  | ✅ | ✅ |  | BytesreasonAccountIdLookupOfTwhoCompactu128tip_value |
    | Tip |  | ✅ | ✅ |  | HashhashCompactu128tip_value |
    | Close tip |  | ✅ | ✅ |  | Hashhash |
    | Slash tip |  | ✅ | ✅ |  | Hashhash |

- ElectionProviderMultiPhase
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Submit unsigned |  |  |  |  | BoxRawSolutionSolutionOfMinerConfigraw_solutionSolutionOrSnapshotSizewitness |
    | Set minimum untrusted score |  |  |  |  | OptionElectionScoremaybe_next_score |
    | Set emergency election result |  |  |  |  | SupportsAccountIdsupports |
    | Submit |  |  |  |  | BoxRawSolutionSolutionOfMinerConfigraw_solution |
    | Governance fallback |  |  |  |  | Optionu32maybe_max_votersOptionu32maybe_max_targets |

- CereDDCModule
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Send data |  |  |  |  | AccountId32sendToBytesdata |

- ChainBridge
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Acknowledge Proposal |  |  |  |  | u64nonceu8srcId[u8;32]rIdCallcall |
    | Add Relayer |  |  |  |  | AccountId32v |
    | Eval Vote State |  |  |  |  | u64nonceu8srcIdCallprop |
    | Reject Proposal |  |  |  |  | u64nonceu8srcId[u8;32]rIdCallcall |
    | Remove Relayer |  |  |  |  | AccountId32v |
    | Remove Resource |  |  |  |  | [u8;32]id |
    | Set Resource |  |  |  |  | [u8;32]idBytesmethod |
    | Set Threshold |  |  |  |  | u32threshold |
    | Whitelist Chain |  |  |  |  | u8id |

- ERC20
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Mint ERC721 |  |  |  |  | AccountId32recipientu256idBytesmetadata |
    | Remark |  |  |  |  | Hashhash |
    | Transfer |  |  |  |  | AccountId32tou128amount |
    | Transfer ERC721 |  |  |  |  | Bytesrecipientu256tokenIdu8destId |
    | Transfer Hash |  |  |  |  | Hashhashu8destId |
    | Transfer Native |  |  |  |  | u128amountBytesrecipientu8destId |

- ERC721
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Mint |  |  |  |  | AccountId32owneru256idBytesmetadata |
    | Burn |  |  |  |  | u256id |
    | Transfer To |  |  |  |  | AccountId32tou256id |

- DDCStaking
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Bond | ✅ | ✅ | ✅ | ✅ | MultiAddresscontrollerCompact<u128>value |
    | Bond extra | ✅ | ✅ | ✅ |  | Compact<u128>amount |
    | Unbond | ✅ | ✅ | ✅ | ✅ | CompactBalanceamount |
    | Withdraw Unbonded | ✅ | ✅ | ✅ |  |  |
    | Store | ✅ | ✅ | ✅ |  | boolfoo |
    | Serve | ✅ | ✅ | ✅ |  | boolfoo |
    | Chill | ✅ | ✅ | ✅ | ✅ |  |
    | Set controller | ✅ | ✅ | ✅ | ✅ | AccountIdLookupOfTcontroller |

- Contracts
    | Name | Nano S | Nano S XL | Nano SP/X | Nesting | Arguments |
    | --- | --- | --- | --- | --- | --- |
    | Call |  |  |  |  | MultiAddressdestCompact<u128>valueCompact<u64>gasLimitOption<Compact<u128>>storageDepositLimitBytesdata |
    | Instantiate |  |  |  |  | Compact<u128>valueCompact<u64>gasLimitOption<Compact<u128>>storageDepositLimitBytescodeHashBytessalt |
    | Instantiate With Code |  |  |  |  | Compact<u128>valueCompact<u64>gasLimitOption<Compact<u128>>storageDepositLimitBytescodeBytesdataBytessalt |
    | Remove Code |  |  |  |  | BytescodeHash |
    | Upload Code |  |  |  |  | BytescodeOption<Compact<u128>>storageDepositLimit |
