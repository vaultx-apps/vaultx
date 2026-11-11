<div align="center">

# VAULTX

### Every curve token, behind one door.

**Live board and trading front-end for Pons bonding-curve tokens on Robinhood Chain.**

[**Launch App**](https://vaultx-apps.github.io/vaultx/) · [**Swap**](https://vaultx-apps.github.io/vaultx/#/swap) · [**Launchpads**](https://vaultx-apps.github.io/vaultx/#/launchpads) · [**Portfolio**](https://vaultx-apps.github.io/vaultx/#/portfolio) · [**$VAULTX**](https://vaultx-apps.github.io/vaultx/#/vaultx) · [**Docs**](https://vaultx-apps.github.io/vaultx/#/docs) · [**Report an Issue**](https://github.com/vaultx-apps/vaultx/issues)

</div>

---

## Overview

VaultX is a Web3 application focused on token discovery, bonding-curve activity, and token trades on **Robinhood Chain**.

The platform brings Pons launchpad token data, token lifecycle information, and market-oriented tools together in one responsive interface. VaultX is built to make emerging markets easier to explore while clearly distinguishing available on-chain evidence from estimates or unavailable data.

> **Project status:** The application is under active development. Some features require supported contracts, configured data providers, and a connected wallet. Displayed market data can be delayed or unavailable.

## Platform Features

| Feature | Description |
| --- | --- |
| **Live Token Discovery** | Browse every Pons launch with search, sorting, and lifecycle filters. |
| **Bonding-Curve Lifecycle** | Follow tokens through **On Curve**, **Graduating**, and **Surfaced** stages. |
| **Buy & Sell the Curve** | Trade directly against the bonding curve at its constant-product price, including the curve's real **3.8% input fee**. No VaultX markup. |
| **Graduation Tracking** | A token graduates at **4.2 ETH** real reserve, then keeps trading on its Uniswap pool (linked via DexScreener). |
| **Swap Interface** | A dedicated swap view with a searchable token picker, using the same live token list and the same quoting as the detail view. |
| **Launchpads** | Pons at a glance: live launch stats and the same token grid. |
| **Portfolio** | Connect a wallet and see the curve tokens it actually holds, valued at live curve prices (ETH + USD), with a total-value summary. |
| **$VAULTX Information** | View the project token overview. **$VAULTX is not launched: there is no contract address, no price, and nowhere to buy it yet.** |
| **Responsive UI** | Navigate a navy + brass-gold interface that works on desktop and mobile. |
| **RPC Resilience** | Three Robinhood RPC endpoints with automatic failover and a stale-data banner, so one failing endpoint never blanks the board. |

Market metrics and displayed statuses depend on network conditions, provider availability, and the scope of the underlying checks.

## Explore the App

| Section | URL | Purpose |
| --- | --- | --- |
| Token Discovery | [vaultx-apps.github.io/vaultx](https://vaultx-apps.github.io/vaultx/) | Live tokens, lifecycle filters, and the token board |
| Swap | [#/swap](https://vaultx-apps.github.io/vaultx/#/swap) | Token swap interface |
| Launchpads | [#/launchpads](https://vaultx-apps.github.io/vaultx/#/launchpads) | Supported launchpad information |
| Portfolio | [#/portfolio](https://vaultx-apps.github.io/vaultx/#/portfolio) | Wallet holdings valued at live curve prices |
| $VAULTX | [#/vaultx](https://vaultx-apps.github.io/vaultx/#/vaultx) | Project token overview (coming soon) |
| Documentation | [#/docs](https://vaultx-apps.github.io/vaultx/#/docs) | Curve mechanics, fee, graduation, and risks |

## Contracts on Robinhood Chain

VaultX reads live data from the **Pons** protocol contracts on Robinhood Chain. These are the protocol addresses the site uses — VaultX itself deploys no contracts:

```text
Pons V2 factory:  0x7ed598bcef8bd9edd8c97a195c6d13f40801ec7e
Fee Escrow:       0xd3AFEB2a57f70eF218Aa82451c51B2fb0416Ac9e
Fee policy/hook:  0xE5e702641Ea86F4ae6cC3cDaeD2B886f976Be044
