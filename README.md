# PQ Open PGP

**PQ Open PGP** is a project that implements the OpenPGP standard with Post-Quantum Cryptography (PQC) algorithms. This standard is proposed by the **IETF (Internet Engineering Task Force)** and is being developed to be resilient against attacks from quantum computers.

- **Reference**: [IETF Draft - PQ Open PGP](https://www.ietf.org/archive/id/draft-ietf-openpgp-pqc-07.html)

## Table of Contents

- [PQ Open PGP](#pq-open-pgp)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Installation](#installation)
    - [Install CafeOBJ](#install-cafeobj)
  - [How to check flow protocol](#how-to-check-flow-protocol)
  - [How to verify the property](#how-to-verify-the-property)
  - [Author](#author)

## Introduction

PQ Open PGP provides a security solution for encrypting and transmitting sensitive data using quantum-resistant algorithms. This project offers algorithms that are not vulnerable to quantum computer attacks, ensuring data protection for the future.

## Installation

To use PQ Open PGP and the IPSG tool, you'll need to install **CafeOBJ** and **IPSG Tool**. Follow the steps below for installation.

### Install CafeOBJ

CafeOBJ is a high-level, executable specification language that is used to define and simulate models for cryptographic systems in the PQ Open PGP framework.

1. Visit the official CafeOBJ website: [CafeOBJ Download](https://cafeobj.org/download/)
2. Follow the installation instructions based on your operating system:
   - For **macOS** and **Linux**, you can follow the installation guides and download the proper binaries.
   - For **Windows**, you may need to use a virtual machine or subsystem to run CafeOBJ.
   
   **Example on macOS** (via Homebrew):
   ```bash
   brew install cafeobj

### Install IPSG Tool
To get started, clone the IPSG Tool repository from GitHub:

```bash
git clone https://github.com/duongtd23/IPSG-tool.git
```

## How to check flow protocol
1. Run command to start **cafeobj**
```
    cafeobj
```
2. Run file to check flow
```
    in check
```

## How to verify the property
1. Run command to start **IPSG Tool**
```
    ./maude -allow-files <folder IPSG>/IPSG-tool/ipsg.maude
```
2. Load the specification file and the invariant file
```
    load pq.cafe .
    load invariants.cafe .
```
3. Run proof files
```
    load /inputs/*.cafe .
```

## Author
- HOANG Trong Binh
- Github: https://github.com/hoangtrongbinh1111