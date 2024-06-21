# SYSTEX2024 Repository

Welcome to the SYSTEX2024 GitHub repository! This repository contains resources and materials related to my master’s thesis in IBM & ETH Zurich, which was accepted for presentation at the SYSTEX2024 workshop.

## Contents

- **drawio/**: Contains diagrams and flowcharts created using draw.io for the thesis presentation.
- **Artifact.md**: Documentation and description of the artifacts used in the thesis.
- **systex24-final56.pdf**: The final version of the document submitted for SYSTEX2024.

## Abstract
Blockchain technology offers decentralized security but fails to ensure data confidentiality due to its inherent data replication across all network nodes. To address these confidentiality challenges, integrating blockchains with Trusted Execution Environments (TEEs), such as Intel SGX, offers a viable solution. This approach, by encrypting all data outside the SGX enclave and making them unrecognizable to untrusted network nodes, ensures secure processing of data and computations within TEEs. Fabric Private Chaincode (FPC), an enhancement of Hyperledger Fabric, demonstrates this integration by securing smart contracts in enclaves, thereby enhancing confidentiality. However, FPC's reliance on states stored on the blockchain introduces vulnerabilities, especially to rollback attacks. This work provides a detailed analysis of rollback attacks in FPC, evaluates existing protection mechanisms, and proposes a solution: a Merkle Tree approach implemented in an FPC application named Secret Keeper. Through experimental validation, this solution shows significant security enhancements against rollback attacks within FPC contexts.
