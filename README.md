# RetailCore

**RetailCore ($RTC) - Interoperable Cashback Protocol**

![RetailCore Executive Summary](docs/project/RTC_single_Page.png)

## Overview

RetailCore ($RTC) is a blockchain-based cashback protocol that establishes **interoperable cashback** across an ecosystem of partner retailers. By tokenising rewards, we transform an illiquid liability into a digital asset that can be used at any partner in the network, increasing customer engagement and retention within the ecosystem.

## Executive Summary

For detailed information about the RetailCore protocol, please refer to the [Executive Summary PDF](docs/project/Resumo%20Executivo_%20RetailCore%20($RTC)%20-%20Protocolo%20de%20Cashback%20Interoperável.pdf).

## Business Problem

The loyalty and retail market is hindered by the inefficiency and low liquidity of traditional points programmes. Statistics indicate that a significant portion of loyalty points expire unused, representing an unrealised liability for companies and frustration for consumers.

The central problems are:
- **Lack of interoperability**: Points are locked to a single retailer
- **Absence of immediate liquidity**: Traditional points cannot be easily converted or used

## Solution

RetailCore addresses these issues by creating a tokenised reward system that:
- Enables cashback to be used across all partner retailers
- Provides immediate liquidity through tokenisation
- Implements deflationary mechanisms to manage supply
- Encourages circulation within the retail ecosystem

## Token Structure (Tokenomics)

The $RTC token is designed as a **deflationary utility token** with an on-chain expiration mechanism to manage reward liabilities and incentivise circulation.

### Token Details

- **Name:** RetailCore
- **Ticker:** $RTC
- **Type:** ERC-20 with expiry extension. The token utilises the interface proposed in [EIP-7818](https://eips.ethereum.org/EIPS/eip-7818) (Expiry Management) to track the Time-To-Live (TTL) of each batch.

### Minting

- Token emission is strictly linked to confirmation of a valid purchase
- To mitigate chargeback and fraud risks, minting is followed by a vesting period of up to **90 days**
- Tokens only become usable after this vesting period

### Cashback Rate

- Dynamically defined by each partner retailer
- Flexible rate ranging from **0.1% to 99.9%** of purchase value

### Validity (TTL - Time-To-Live)

- The $RTC token has an intrinsic and programmable validity period
- Tokens expire and are automatically **burned** if not used within **90 days** after their emission date (after vesting completion)
- This deflationary mechanism manages supply and forces circulation

## Incentive Mechanics (Game Theory)

The primary objective of $RTC tokenomics is to **incentivise reuse and circulation of the token within the retail ecosystem**, ensuring value remains in the network (Internal Liquidity).

| Incentive Rule | Description | Conversion Rate | Economic Impact |
|:---------------|:------------|:---------------|:----------------|
| **Network Usage Rule** | Using $RTC to purchase products or services at any partner retailer | **1 $RTC = 1 Fiat Currency Unit** (1:1) | **Maximum incentive** for consumers to spend tokens in retail, increasing the Gross Merchandise Volume (GMV) of the network |
| **Cashout Rule** | Converting $RTC to fiat currency (withdrawal/bank transfer) | **1 $RTC = 0.70 Fiat Currency Unit** (0.7:1) | **30% disincentive** (discount) for immediate sale. Promotes value retention in the network and inhibits selling pressure in the market |

## Technical Differentiator: EIP-7818

The technical implementation of $RTC leverages the proposed **EIP-7818** for on-chain management of expiration dates and balances.

This approach enables:

- **User Transparency:** Compatible wallets can read the EIP-7818 interface and natively display the exact balance, emission date, and crucially, the **expiration date** of each batch of $RTC tokens held
- **Accurate Accounting:** The protocol manages automatic burning of expired tokens, ensuring the circulating supply reflects only real and active liabilities
- **Audit Efficiency:** Facilitates auditing of reward liabilities for retailers, as the validity state is maintained in a decentralised and immutable manner

## Key Features

- ✅ **Interoperability**: Use cashback across all partner retailers
- ✅ **Tokenisation**: Convert illiquid points into tradeable digital assets
- ✅ **Deflationary Design**: Automatic expiration and burning mechanism
- ✅ **Transparent Accounting**: On-chain tracking via EIP-7818
- ✅ **Fraud Protection**: 90-day vesting period
- ✅ **Network Incentives**: Economic mechanisms to keep value in the ecosystem

## Conclusion

RetailCore ($RTC) is not just a loyalty programme; it is a tokenised liquidity infrastructure for retail. Its deflationary design and robust game theory ensure it fulfils the promise of an interoperable cashback asset, maintaining value within the ecosystem and incentivising consumption.

## License

This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for details.

---

**Date:** 16 Feb 2026  
**Prepared by:** Roberto Pavusa Junior  
**Status:** Tokenomics Proposal
