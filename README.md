# Ripple: Tokenized Creator Funding Platform

![Ripple Web3 Creator Economy](https://img.shields.io/badge/Ripple-Web3_Creator_Economy-blue)
![License: MIT](https://img.shields.io/badge/license-MIT-green)
![Ethereum L2 Base](https://img.shields.io/badge/Ethereum-L2_Base-3C3C3D)
![Next.js 14](https://img.shields.io/badge/Next.js-14-black)
![Go 1.21+](https://img.shields.io/badge/Go-1.21%252B-00ADD8)
![NestJS 10](https://img.shields.io/badge/NestJS-10-E0234E)

Ripple is a Web3-native alternative to Patreon that enables continuous, tokenized funding for creators through streaming payments. Creators receive sustainable income streams while supporters invest directly in creator success with real-time yield distribution.

## 🎯 The Problem with Traditional Platforms
Current creator funding platforms suffer from:
- **Batch payments**: Monthly or weekly payouts instead of continuous income
- **High fees**: 5-12% platform fees eating into creator revenue
- **Centralized control**: Platforms can demonetize creators arbitrarily
- **No ownership**: Supporters don't benefit from creator growth
- **Geographic restrictions**: Limited payment methods and country availability

## ✨ Ripple's Solution
Ripple transforms creator funding through:
- **Streaming Payments**: Real-time, continuous revenue flow via Drips protocol
- **Tokenized Ownership**: ERC-1155 vaults representing creator membership tiers
- **Lower Fees**: 2% platform fee with yield distribution to token holders
- **Global Access**: Crypto-native with optional fiat on/off ramps
- **Transparent Economics**: All transactions on-chain, verifiable by anyone

## 🏗️ Architecture Overview
### Layer 1: Smart Contracts (Ethereum L2 - Base)
Gas-efficient, secure contracts that power the platform:
- `RippleFactory.sol`: Creator vault deployment factory
- `CreatorVault.sol`: ERC-1155 vault for each creator (membership NFTs)
- `RippleToken.sol`: Platform utility token (ERC-20) for governance
- `RevenueSplitter.sol`: Automated royalty distribution
- `DripsAdapter.sol`: Interface to Drips v2 streaming protocol

### Layer 2: Backend Services (Go + Node.js)
High-performance, scalable backend with clear separation:
- **Go API Service**: Core payment processing and blockchain interactions
- **NestJS Business Service**: User management, content, and creator features
- **Indexer Service**: Real-time blockchain event indexing
- **Notification Service**: Real-time alerts and webhooks
- **Payment Service**: Fiat ↔ Crypto bridge with Stripe integration

### Layer 3: Frontend Application (Next.js 14 + TypeScript)
Modern, responsive web interface:
- **Creator Dashboard**: Analytics, content management, earnings tracking
- **Supporter Interface**: Creator discovery, subscription flows, content feed
- **Web3 Integration**: Wallet connection (Privy/Web3Modal), transaction signing
- **Real-time Updates**: Live payment streams and notification system

### Layer 4: Data & Infrastructure
Reliable data persistence and storage:
- **PostgreSQL**: Primary relational database for user data
- **Redis**: Caching, session management, and real-time features
- **IPFS (via Pinata)**: Decentralized content storage
- **The Graph**: Indexed blockchain data for efficient queries

### Layer 5: External Integrations
Best-in-class third-party services:
- **Stripe**: Fiat payment processing and on/off ramps
- **Privy**: Embedded wallets and simplified Web3 onboarding
- **Resend**: Transactional email delivery
- **PostHog**: Product analytics and user behavior tracking
- **Sentry**: Error monitoring and performance tracking

## 🚀 Quick Start
### Prerequisites
- Node.js 18+ and npm/yarn/pnpm
- Go 1.21+
- Docker and Docker Compose
- MetaMask or any Web3 wallet
- Base Sepolia testnet ETH (for testing)



---
**Ripple**: Empowering creators with continuous, community-driven funding. Join the streaming economy revolution.