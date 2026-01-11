# 🎮 iRC Official Token - Multi-Game Ecosystem Currency

## Overview

**iRC (iRunCrypto)** is the official utility token powering the iRunCrypto.com gaming ecosystem. It serves as the unified currency across 5 distinct games:

1. **FiveM Server** - Real-time multiplayer (high-velocity transactions)
2. **Turn-Based Game 1** - Strategic gameplay
3. **Turn-Based Game 2** - Strategic gameplay
4. **Turn-Based Game 3** - Strategic gameplay
5. **Turn-Based Game 4** - Strategic gameplay

## Token Specifications

| Property | Value |
|----------|-------|
| **Token Name** | iRC Token |
| **Symbol** | iRC |
| **Blockchain** | Solana |
| **Token Standard** | SPL Token |
| **Total Supply** | 5,000,000,000 (5 Billion) |
| **Decimals** | 6 |
| **Initial Price Target** | $0.001 USD |

## Token Allocation

```
┌─────────────────────────────────────────────────────────────────┐
│                    iRC TOKEN ALLOCATION                         │
│                     5,000,000,000 Total                         │
├─────────────────────────────────────────────────────────────────┤
│  ██████████████████████████████  55%  Ecosystem Vault           │
│  ████████████                    15%  DEX Liquidity (Raydium)   │
│  ████████████                    15%  Team & Development        │
│  ████████                        10%  Marketing & Partnerships  │
│  ████                             5%  Community Airdrops        │
└─────────────────────────────────────────────────────────────────┘
```

## Project Structure

```
iRC Official Token/
├── README.md                    # This file
├── TOKENOMICS.md               # Detailed economic model
├── Official Token Image.png    # Token logo/branding
├── config/
│   ├── token-metadata.json     # SPL token metadata
│   └── allocation-wallets.json # Multi-sig wallet addresses
├── contracts/
│   ├── vesting/
│   │   ├── team-vesting.md     # Team token vesting schedule
│   │   └── vault-emission.md   # Vault release mechanism
│   └── treasury/
│       └── multi-sig-setup.md  # Multi-signature treasury guide
├── launch/
│   ├── raydium-launch-guide.md # DEX liquidity pool setup
│   ├── lp-lock-guide.md        # LP token locking instructions
│   └── launch-checklist.md     # Pre-launch verification
├── integrations/
│   ├── fivem-api-spec.md       # FiveM server integration
│   ├── turnbased-api-spec.md   # Turn-based games integration
│   └── vault-faucet-sink.md    # Token flow architecture
└── security/
    ├── audit-requirements.md   # Smart contract audit needs
    └── multi-sig-policy.md     # Treasury access policies
```

## Quick Start

1. **Review Tokenomics** → See `TOKENOMICS.md`
2. **Prepare Wallets** → See `config/allocation-wallets.json`
3. **Mint Token** → See `launch/launch-checklist.md`
4. **Lock Vesting** → See `contracts/vesting/`
5. **Launch on Raydium** → See `launch/raydium-launch-guide.md`
6. **Integrate Games** → See `integrations/`

## Critical Reminders

⚠️ **Never release team tokens without vesting lock**  
⚠️ **Always lock LP tokens for minimum 6-12 months**  
⚠️ **Vault tokens must return via sinks (in-game purchases)**  
⚠️ **Use multi-sig for all treasury operations**

---

**Website:** iRunCrypto.com  
**Created:** January 2026
