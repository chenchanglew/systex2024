# SYSTEX2024 Repository

[![Static Badge](https://systex24.github.io/img/systexbadges-available.svg)](https://systex24.github.io/artifact.html)

Welcome to the SYSTEX2024 GitHub repository! This repository contains resources and materials related to my master’s thesis in IBM & ETH Zurich, which was accepted for presentation at the SYSTEX2024 workshop.
Paper title: Revisiting Rollbacks on Smart Contracts in TEE-protected Private Blockchains.


## Contents

- **drawio/**: Contains diagrams and flowcharts created using draw.io for the thesis presentation.
- **systex24-final56.pdf**: The final version of the document submitted for SYSTEX2024.

## Abstract
Blockchain technology offers decentralized security but fails to ensure data confidentiality due to its inherent data replication across all network nodes. To address these confidentiality challenges, integrating blockchains with Trusted Execution Environments (TEEs), such as Intel SGX, offers a viable solution. This approach, by encrypting all data outside the SGX enclave and making them unrecognizable to untrusted network nodes, ensures secure processing of data and computations within TEEs. Fabric Private Chaincode (FPC), an enhancement of Hyperledger Fabric, demonstrates this integration by securing smart contracts in enclaves, thereby enhancing confidentiality. However, FPC's reliance on states stored on the blockchain introduces vulnerabilities, especially to rollback attacks. This work provides a detailed analysis of rollback attacks in FPC, evaluates existing protection mechanisms, and proposes a solution: a Merkle Tree approach implemented in an FPC application named Secret Keeper. Through experimental validation, this solution shows significant security enhancements against rollback attacks within FPC contexts.

## Artifact


### Requirements:

- **Hyperledger Fabric v2.3.3**: [GitHub link](https://github.com/hyperledger/fabric/releases/tag/v2.3.3)
- **FPC branch go-support-preview**: [GitHub link](https://github.com/chenchanglew/fabric-private-chaincode/tree/go-support-preview)

### My Implementation

- **FPC Application Secret Keeper**:
  - The implementation of the secret keeper mentioned in section 2.5
  - Github Branch: [Secret Keeper Go](https://github.com/chenchanglew/fabric-private-chaincode/tree/thesis/rollback-protection-zac/samples/chaincode/secret-keeper-go)
  - Permanent link: [Secret Keeper Go](https://github.com/chenchanglew/fabric-private-chaincode/tree/b7821e80aa752514f5419b8f567ce3c77ce02c34/samples/chaincode/secret-keeper-go)
  - Loom demonstration video: [Watch here](https://www.loom.com/share/e3dca62f8df849229e2c6414fd374289?sid=473acda1-92ac-4ad6-89c4-ddb2f5786dd5)

- **Fabric Malicious Peer**:
  - The implementation of the malicious peer mentioned in section 2.5
  - Github Branch: [Malicious Peer](https://github.com/chenchanglew/fabric/tree/feature/malicious-peer)
  - Permanent link: [Malicious Peer](https://github.com/chenchanglew/fabric/tree/4a34c84a0c42c027471cb3d005550eb01dc9e2a5/)
  - Loom demonstration video: [Watch here](https://www.loom.com/share/e540bf6395f94ab8ba547bd43942d063?sid=b32de7ea-e5d7-43ef-9e06-bf11b3cfc6ff)

- **FPC Rollback Protection Main Branch**:
  - The implementation of all the FPC rollback protection methods mentioned in section 4.
  - Github Branch: [Rollback Protection](https://github.com/chenchanglew/fabric-private-chaincode/tree/thesis/rollback-protection-zac)
  - Permanent link: [Rollback Protection](https://github.com/chenchanglew/fabric-private-chaincode/tree/b7821e80aa752514f5419b8f567ce3c77ce02c34/)

- **SKVS Solution**:
  - The implementation of the SKVS solution mentioned in section 2.7
  - GitHub Pull Request: [SKVS Solution](https://github.com/chenchanglew/fabric-private-chaincode/pull/3)
  - Permanent link: [SKVS Solution](https://github.com/chenchanglew/fabric-private-chaincode/commit/f93e072f69b35734dba5a8de9f91b1c89fcfb7d4) 
  - Loom demonstration video: [Watch here](https://www.loom.com/share/4790cd0cba9e4433879083b41158d42d?sid=a0f367e7-dc49-4065-926d-df7b2fbf55a1)

- **TLE Solution**:
  - **Fabric TLE Support**:
    - The implementation of TLE support in Fabric mentioned in section 2.7
    - GitHub Branch: [Fabric TLE Support](https://github.com/chenchanglew/fabric/tree/feature/support-TLE)
    - Permanent link: [Fabric TLE Support](https://github.com/chenchanglew/fabric/tree/2bd56f3b43c311edc78c5903ac75e7c76d2ec61f/)
  - **FPC TLE Implementation**:
    - The implementation of TLE in FPC mentioned in section 2.7
    - GitHub Branch: [FPC TLE Implementation](https://github.com/chenchanglew/fabric-private-chaincode/tree/thesis/tle-solution)
    - Permanent link: [FPC TLE Implementation](https://github.com/chenchanglew/fabric-private-chaincode/tree/9f9876451c32f31cb064d56bdcd302547869717d)
  - Loom demonstration video: [Watch here](https://www.loom.com/share/4e8814304bcd49c9860861be524febbd?sid=c64b4cdb-0ae3-4125-93af-f369349f11f8)

- **Merkle Tree Approach**:
  - **Fabric Merkle Tree Support**:
    - The implementation of Merkle Tree support in Fabric in section 3.2
    - GitHub Branch: [Fabric Merkle Tree Support](https://github.com/chenchanglew/fabric/tree/feature/support-merkle)
    - Permanent link: [Fabric Merkle Tree Support](https://github.com/chenchanglew/fabric/tree/98c7b36cb98cd14ac8926b89a5e688e08787d03b)
  - **FPC Merkle Tree Implementation**:
    - The implementation of the Merkle Tree in FPC.
    - GitHub Branch: [FPC Merkle Tree Implementation](https://github.com/chenchanglew/fabric-private-chaincode/tree/thesis/merkle-solution)
    - Permanent link: [FPC Merkle Tree Implementation](https://github.com/chenchanglew/fabric-private-chaincode/tree/abb0ed62abaa0fb55a255a092c6f672cc3df4fe2)
  - Loom demonstration video: [Watch here](https://www.loom.com/share/632e389fc03540c4ae1de35440ccbbd1?sid=29d97578-61f5-43a8-b791-6ee5cce450ec)
