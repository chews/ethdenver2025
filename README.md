# Safest Sofar - Hardware Wallet and dapprunner

## Overview

In response to the recent security breach of app.safe.global where North Korean hackers compromised a developer's laptop and exposed AWS credentials, this project offers a comprehensive security solution for Gnosis Safe wallets. The implementation runs a complete Gnosis Safe infrastructure stack on a Raspberry Pi 5, creating a self-contained, air-gapped transaction signing environment that operates independently from vulnerable web interfaces.

## Architecture

The system architecture features multiple security layers, beginning with a locally hosted version of the Gnosis Safe software that eliminates dependency on potentially compromised web services. This allows users to create, sign, and broadcast transactions directly from the Raspberry Pi without exposing sensitive operations to internet-connected services.

## Security Components

The security cornerstone is the integrated Zymbit HSM6 (Hardware Security Module), which provides military-grade key protection. This dedicated hardware stores all private signing keys in a physically isolated, tamper-resistant environment with features including:

- Physical tamper detection that can automatically wipe keys if breached
- Encrypted key storage with dedicated secure processing
- Hardware-based random number generation for cryptographic operations
- Secure authentication mechanisms before allowing signature creation

## Features

The implementation includes a custom interface for transaction management and monitoring, with optional multi-signature requirements configurable for additional security. All communications between the Raspberry Pi and external networks are encrypted and can be configured to route through TOR for enhanced privacy.

## Security Advantages

This solution effectively mitigates the attack vector exploited in the recent breach by decoupling critical signing operations from potentially compromised web infrastructure, creating a robust, self-sovereign alternative for managing digital assets.