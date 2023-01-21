---
id: dao-comprehension-check
title: "Arbitrum DAO: Comprehension check"
sidebar_label: Comprehension check
description: todo:qqq
---

import DraftExpectationsPartial from '@site/docs/partials/_draft-expectations-partial.md'; 

<DraftExpectationsPartial />

todo - clean this up, possibly use the spoiler styles to hide answers, consider squishing the Scenario / Question into a single line.

Use the following scenarios to test your comprehension of the different components of the Arbitrum DAO protocol, such as the Security Council, AIPs, on-chain and off-chain actions. By exercising your understanding of these scenarios, you'll be better equipped to confidently navigate the process, technology, and governance proposals that support the Arbitrum DAO.


#### Scenario 1: You have an idea that you'd like to propose to the Arbitrum DAO

**Question**: What's the first step you should take to propose an idea to the Arbitrum DAO?

**Answer**: The first step is to submit the idea as an Arbitrum Improvement Proposal (AIP) on the public governance forum (todo) and discuss/debate it for 1 week. This is known as the Temperature Check phase and is optional but strongly recommended as a due-diligence governance best practice.


#### Scenario 2: A security emergency arises on one of the Arbitrum DAO-governed chains

**Question**: How can the DAO respond to the security emergency?

**Answer**: The Security Council, a committee of 12 members who are signers of a multi-sig wallet, should implement the software upgrade (or perform whatever other action is required) immediately in order to remedy the situation. This is known as an Emergency Action and requires a 9-of-12 approval from the Security Council. The Security Council shouldn't use its power to perform Emergency Actions except in a true security emergency, such as a critical vulnerability that could significantly compromise the integrity, confidentiality, or availability of a chain governed by the Arbitrum DAO. After performing an Emergency Action, the Security Council must issue a full transparency report to explain what was done and why the Emergency Action was justified.


#### Scenario 3: You want to propose a change to the system parameters of one of the Arbitrum DAO-governed chains

**Question**: What's the process for proposing and implementing this change?

**Answer**: The process for proposing and implementing changes to system parameters is as follows:

1. Submit the proposal as an AIP on the public forum and discuss/debate it for 1 week (Temperature Check phase)
2. The AIP moves on to a voting phase where token-holders can vote on the proposal
3. If the proposal passes the vote, it moves on to a delay period before implementation
4. After the delay period, the change can be implemented by the chain owner(s) through a transaction on the blockchain.

Note that the Security Council may also approve and implement routine software upgrades, routine maintenance, and other parameter adjustments in a non-emergency setting, which require a 7-of-12 approval in order to take effect. This bypasses Phases 1 to 3 of the AIP process and instead directly goes through Phases 4 to 7. This prevents routine upgrades and maintenance from being delayed by the voting and delay phases of the AIP process.


#### Scenario 4: You want to propose a change to the Constitution of the Arbitrum DAO

**Question**: What's the process for proposing and implementing this change?

**Answer**: The process for proposing and implementing changes to the Constitution is as described in the Constitution itself. It involves submitting the proposal as an AIP, and then going through the same voting and delay phases as any other proposal. The proposal must pass with a supermajority of Votable Tokens being voted in favor of the change. Changes to the Constitution must also be ratified by the Security Council with a 7-of-12 approval in order to take effect.


#### Scenario 5: You want to propose a new Arbitrum DAO-governed chain

**Question**: What's the process for proposing and implementing this change?

**Answer**: The process for proposing and implementing a new Arbitrum DAO-governed chain involves submitting the proposal as an AIP, and then going through the same voting and delay phases as any other proposal. The proposal must pass with a supermajority of Votable Tokens being voted in favor of the change. The new chain must also be authorized by the Arbitrum DAO through a corresponding AIP. The new chain must be governed solely by the Constitution and the procedures as described in TODO.


#### Scenario 6: You want to become a member of the Security Council

**Question**: What's the process for becoming a member of the Security Council?

**Answer**: The Security Council has 12 members, who are divided into a July cohort of 6 members, and a January cohort of 6 members. Every year on July 15th, 12:00 UTC, an election starts for the July 6th cohort seats; and every year on January 15th, 12:00 UTC, an election starts for the January 6th cohort seats. To become a member of the Security Council, you would need to be elected through this process.


#### Scenario 7: You want to upgrade the Arbitrum One chain

**Question**: What's the process for upgrading the Arbitrum One chain?

**Answer**: The process for upgrading the Arbitrum One chain involves submitting a proposal as an AIP and going through the same voting and delay phases as any other proposal. The proposal must pass with a supermajority of Votable Tokens being voted in favor of the change. The upgrade must also be approved by the Security Council with a 7-of-12 approval in order to take effect. The chain owner(s) will then perform the upgrade by updating the contract implementation of any of Arbitrum's core protocol [Transparent Upgradeable Proxy contracts](https://developer.arbitrum.io/useful-addresses), and adjusting system parameters (for example: through `setter` methods in the [ArbOwner precompile](https://github.com/OffchainLabs/nitro/blob/master/contracts/src/precompiles/ArbOwner.sol)).

It's important to note that the upgrade should be thoroughly tested and reviewed by the community and experts in the field before being proposed and implemented. Any upgrade should also be compliant with the applicable laws, in particular sanctions-related regulations.


#### Scenario 11: The Arbitrum DAO experiences a season of voter apathy.

**Question**: Will this prevent work from being done on the chains that the Arbitrum DAO owns?

**Answer**: No, voter apathy won't prevent work from being done on the chains that the Arbitrum DAO owns. The Constitution allows for off-chain actions to be taken, which don't require the approval of token holders. The Security Council has the power to perform Emergency Actions with a 9-of-12 approval, which can be used to address critical issues that cannot wait for voter approval. While voter participation is important for the proper functioning of the DAO, the Constitution has built-in mechanisms to ensure that work can continue to be done even in the event of low voter turnout.

Note that voter apathy could have an impact on the governance of the DAO, and certain decisions and actions might not be as representative of the community's collective will if voter turnout is low.


#### Scenario 12: You've claimed $ARB tokens, but you don't have time to actively participate in Arbitrum DAO's governance.

**Question**: What options do you have?

**Answer**: If you've claimed $ARB tokens but don't have time to actively participate in the Arbitrum DAO's governance, you have a few options:

1. You can delegate your voting rights to another member of the community who you trust to make decisions that align with your interests. See TODO
2. You can hold onto your $ARB tokens and vote when you have the time, but please note that some important decisions may have already been made.
3. You can sell or transfer your $ARB tokens to another member of the community who is more active.

While participating in governance is an important aspect of being a DAO member, it's not mandatory. As long as you hold $ARB tokens, you have a right to participate in the Arbitrum DAO's governance protocol, but you also have the right to choose not to participate. No pressure :).


#### Scenario 13: You want to propose a change to the way that unclaimed airdropped $ARB tokens are distributed

**Question**: What's the process for proposing and implementing this change?

**Answer**: The process for proposing and implementing changes to the distribution of unclaimed airdropped $ARB tokens involves submitting a proposal as an AIP and going through the same voting and delay phases as any other proposal. The proposal must pass with a supermajority of Votable Tokens being voted in favor of the change. Additionally, the change must also be approved by the Security Council with a 7-of-12 approval in order to take effect. The distribution of unclaimed airdropped $ARB tokens should be thoroughly evaluated and reviewed by the community and experts in the field before being proposed and implemented.


#### Scenario 14: A malicious whale purchases a majority of Votable Tokens.

**Question**: Can the whale destroy the DAO?

**Answer**: A malicious whale purchasing a majority of Votable Tokens doesn't necessarily mean that the DAO can be destroyed. The Constitution has built-in mechanisms to prevent any single entity from having too much control over the DAO. For example, the Security Council can perform Emergency Actions that require a 9-of-12 approval, which can be used to address critical issues that cannot wait for voter approval. The Constitution also allows for off-chain actions to be taken, which don't require the approval of token holders.

It's worth noting that this theoretical malicious whale's ownership of the majority of Votable Tokens will give them significant influence over the governance of the Arbitrum DAO, and might make it harder for the other members to pass their proposals. In such cases, the community should consider different ways to mitigate the influence of a single entity such as token-curbing mechanisms, or implementing a cap on the maximum percentage of tokens an individual or an entity can own. Please note that this scenario is a risk for any decentralized autonomous organization (DAO) and it's important for the community to be aware of it and have measures in place to mitigate it.


#### Scenario 15: A governance proposal passes that you voted against.

**Question**: What options do you have?

**Answer**: If a governance proposal passes that you voted against, you have a few options:

 1. You can accept the outcome and continue to participate in the DAO. 
 2. You can engage in further discussions and debates on the community forum to express your dissenting opinion and try to sway others to your point of view. 
 3. You can propose a new AIP that addresses the issues you have with the proposal that passed and try to get it passed through the voting process. 
 4. You can choose to disengage from the DAO altogether and sell your Votable Tokens before the proposal takes effect. This is facilitated by the time delay between the proposal passing and the proposal taking effect.


### Conclusion

We hope that this document has been helpful as a self-assessment and study aid. If you have any questions or suggestions, please feel free to reach out to us on the community forum (TODO) or on Discord (TODO). We're always happy to help :).