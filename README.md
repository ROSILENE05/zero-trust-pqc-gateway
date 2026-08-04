# Zero-Trust-PQC-Gateway
# Software-Defined Zero-Trust Gateway with PQC (ML-KEM)

## Architecture Overview
<img width="1024" height="559" alt="Design_roteadorGateway" src="https://github.com/user-attachments/assets/66b3c842-deaf-45a0-a969-0268b9e7b605" />

## About the Project
This repository is a Proof of Concept (PoC) demonstrating a sovereign network architecture. It abstracts hardware dependencies to focus on two core cybersecurity paradigms:
1. **Zero-Trust Network Access (ZTNA):** A default-deny rule engine simulating eBPF packet interception.
2. **Post-Quantum Cryptography (PQC):** A simulation of Key Encapsulation Mechanisms (KEM) to protect symmetric tunnel keys against "Harvest Now, Decrypt Later" quantum attacks.

## How to Run
This PoC is built in pure Python and requires zero installation. 
You can run it directly in your browser:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([LINK_DO_SEU_COLAB_AQUI](https://github.com/ROSILENE05/zero-trust-pqc-gateway/blob/main/Gateway_ZeroTrust_PQC_PoC.ipynb))

## Core Modules
- **Rule Engine:** Prevents IP spoofing and unauthorized node attachment.
- **Audit Ledger:** Cryptographic hashing of all access logs.
- **KEM Handshake:** Ephemeral keypair generation, encapsulation, and decapsulation logic.
