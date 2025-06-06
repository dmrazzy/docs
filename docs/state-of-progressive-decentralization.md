---
id: state-of-progressive-decentralization
title: The state of Arbitrum's progressive decentralization
sidebar_label: State of decentralization
description: Learn about the state of Arbitrum's progressive decentralization.
dao_author: dzgoldman
dao_sme: dzgoldman
---

import DraftExpectationsPartial from '@site/docs/partials/\_draft-expectations-partial.md';

<DraftExpectationsPartial />

<a data-quicklook-from='progressive-decentralization'>Progressive decentralization</a> is the process of gradually increasing the decentralization of a system over time. This document details the current state of progressive decentralization for the <a data-quicklook-from='arbitrum-one'>Arbitrum One</a> and <a data-quicklook-from='arbitrum-nova'>Arbitrum Nova</a> chains, the two chains currently governed by the <a data-quicklook-from='arbitrum-dao'>Arbitrum DAO</a>.

### The components of Arbitrum's progressive decentralization

The following components determine the degree of decentralization for Arbitrum One and Arbitrum Nova:

1. [**Chain ownership**](#1-chain-ownership)
2. [**Validation decentralization status**](#2-validation-decentralization-status)
3. [**Sequencer ownership**](#3-sequencer-ownership)
4. [**Data Availability Committee ownership**](#4-data-availability-committee-ownership)

Let's evaluate the current status of these components for both Arbitrum One and Arbitrum Nova, beginning with <a data-quicklook-from='arbitrum-chain-owner'>chain ownership</a>.

### 1. Chain ownership

- **Description**: A chain's "owner" has the ability to change the protocol in various ways, including upgrading the core smart contracts, setting system parameters, and pausing the system.
- **Current status**: **Governed by Arbitrum DAO**. Chain ownership of both Arbitrum One and Arbitrum Nova is under the control of the Arbitrum governance system. The Arbitrum Decentralized Autonomous Organization (DAO), made up of <a data-quicklook-from='arb'>`$ARB`</a> token-holders and <a data-quicklook-from='delegate'>delegates</a>, can carry out chain-owner operations through governance votes. The <a data-quicklook-from='security-council'>Security Council </a> can also carry out chain-owner operations; it can act quickly through a 9 of 12 <a data-quicklook-from='multisignature-wallet'>multisig wallet</a>, but only in critical emergency situations. The Security Council can also act slowly through a 9 of 12 multisig wallet in non-emergency situations to carry out routine and minor upgrades, such as minor bug fixes. The members of the Security Council (split by cohort) are <a data-quicklook-from='security-council-election'>elected</a> every six months by the Arbitrum DAO.
- **Risks**:
  - If 9 of the Security Council members are compromised or behave maliciously, the system and users' funds could be compromised.
  - If a malicious proposal is successfully put through DAO governance, or if 9 of the Security Council members are compromised or behave maliciously, the system's safety could be compromised. In either of these cases, users will have several weeks to withdraw their funds back to Ethereum before the proposal takes effect.
- **Changes To Current Status**: The governance system currently has the ability to alter governance itself.

### 2. Validation decentralization status

- **Description**: Validators are responsible for confirming the valid state of the <a data-quicklook-from='arbitrum-chain'>Arbitrum chains</a> back on L1.

| Chain                  | Decentralization&nbsp;Status | Description                                                                                                                                                                                                                                     |
|------------------------|------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Arbitrum&nbsp;One**  | **Permissionless**           | Validation on Arbitrum One now follows the BoLD protocol, any node implementing the BoLD protocol can join. You can learn more about BoLD in this [introduction to BoLD](https://docs.arbitrum.io/how-arbitrum-works/bold/gentle-introduction) |
| **Arbitrum&nbsp;Nova** | **Permissioned**             | Arbitrum Nova remains permissioned as its Data Availability committee is a trusted one                                                                                                                                                         |

- **Risks**: If there is not a single honest active validator, and a malicious validator proposes an invalid state update, the system's safety could be compromised.

### 3. Sequencer ownership

- **Description**: The Sequencer is typically responsible for collecting and ordering users' transactions.
- **Current status**: **Centralized**. The Sequencers for both Arbitrum One and Arbitrum Nova are currently maintained by the Arbitrum Foundation. Governance currently has the power to select new Sequencers.
- **Risks**: The Sequencer has the ability to delay the inclusion of a user's transaction by up to 24 hours and reorder transactions over short time-horizons. The Sequencer, however, cannot compromise the system's safety or prevent a transaction from ultimately being executed.
- **Changes to Current status**: The Arbitrum governance system (see #1) currently has the power to elect a new entity as the Sequencer.

### 4. Data Availability Committee ownership

DACs apply only to <a data-quicklook-from='arbitrum-anytrust-protocol'>Arbitrum AnyTrust</a> chains like Arbitrum Nova
:::note

This applies only to Arbitrum AnyTrust chains like Arbitrum Nova.

:::

- **Description**: AnyTrust chains like Arbitrum Nova rely on a permissioned committee to store the chain's data and provide it on demand.
- **Current status**: 6-member committee. The Arbitrum Nova chain has a 6-party DAC, whose members can be seen [here](#data-availability-committee-members). Governance has the ability to remove or add members to the committee.
- **Risks**: If 5 of the 6 committee members in conjunction with the Sequencer behave maliciously and collude, the safety of the system can be compromised.
- **Changes to Current status**: The Arbitrum governance system (see #1) currently has the power to change the DAC, such as by adding or removing members or modifying the power it has over the system.

### Data Availability Committee members

These are the current members of the 5-of-6 [data availability committee (DAC)](#4-data-availability-committee-dac-ownership) in Arbitrum Nova:

- ConsenSys Software Inc.
- QuickNode, Inc.
- P2P.org
- Google Cloud
- Offchain Labs, Inc.
- Opensea Innovation Labs Private Limited
