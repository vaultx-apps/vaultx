<div align="center">

# VAULTX

### Every curve token, behind one door.

**Live board for Virtuals Protocol agent tokens — market caps, volumes, and curve progress, with trading on app.virtuals.io.**

[**Launch App**](https://vaultx-apps.github.io/vaultx/) · [**Swap**](https://vaultx-apps.github.io/vaultx/#/swap) · [**Launchpads**](https://vaultx-apps.github.io/vaultx/#/launchpads) · [**Portfolio**](https://vaultx-apps.github.io/vaultx/#/portfolio) · [**$VAULTX**](https://vaultx-apps.github.io/vaultx/#/vaultx) · [**Docs**](https://vaultx-apps.github.io/vaultx/#/docs) · [**Report an Issue**](https://github.com/vaultx-apps/vaultx/issues)

</div>

---

## Overview

VaultX is a Web3 application focused on token discovery for **Virtuals Protocol** — the launchpad for AI agent tokens.

The platform brings Virtuals agent-token data, token lifecycle information, and market-oriented tools together in one responsive interface. VaultX reads the public Virtuals API, so the board shows real agent tokens across the chains Virtuals serves (Base, Robinhood, and more) — still on their bonding curve or already graduated. Trading itself happens on Virtuals; every token in VaultX links straight to its market on app.virtuals.io.

> **Project status:** The application is under active development. Displayed market data comes from the Virtuals API and can be delayed or unavailable.

## Platform Features

| Feature | Description |
| --- | --- |
| **Live Token Discovery** | Browse Virtuals agent tokens with search, sorting, and filters by chain and lifecycle status. |
| **Bonding-Curve Lifecycle** | Follow tokens through **On Curve** (still bonding) and **Graduated** (live market) stages. |
| **Market Data** | Market cap and FDV in VIRTUAL, 24h volume, 1h/24h price changes, holder counts, and liquidity — straight from the Virtuals API. |
| **Trade on Virtuals** | Every token detail links to its market on app.virtuals.io, where trading happens. No VaultX markup, no VaultX fee. |
| **Launchpads** | Virtuals Protocol at a glance — the launchpad for AI agent tokens, and the future home of $VAULTX. |
| **Portfolio** | Connect a wallet and see the loaded Virtuals tokens it holds on Base and Robinhood Chain, valued in VIRTUAL (estimate). |
| **$VAULTX Information** | View the project token overview. **$VAULTX is launching on Virtuals Protocol: the official contract address will be published here once the token is live.** |
| **Responsive UI** | Navigate a navy + brass-gold interface that works on desktop and mobile. |
| **Honest Data States** | If the API is unreachable, the board shows a clear error/stale state with retry — never invented data. |

Market metrics and displayed statuses depend on network conditions, provider availability, and the scope of the underlying checks.

## Explore the App

| Section | URL | Purpose |
| --- | --- | --- |
| Token Discovery | [vaultx-apps.github.io/vaultx](https://vaultx-apps.github.io/vaultx/) | Virtuals agent tokens, lifecycle filters, and the token board |
| Swap | [#/swap](https://vaultx-apps.github.io/vaultx/#/swap) | How trading works on Virtuals, with a link to the app |
| Launchpads | [#/launchpads](https://vaultx-apps.github.io/vaultx/#/launchpads) | Virtuals Protocol, the agent-token launchpad |
| Portfolio | [#/portfolio](https://vaultx-apps.github.io/vaultx/#/portfolio) | Wallet holdings of loaded Virtuals tokens, valued in VIRTUAL |
| $VAULTX | [#/vaultx](https://vaultx-apps.github.io/vaultx/#/vaultx) | Project token overview (launching on Virtuals) |
| Documentation | [#/docs](https://vaultx-apps.github.io/vaultx/#/docs) | Virtuals curve mechanics, graduation, and risks |

## Data Source

VaultX reads live data from the **public Virtuals API**:

- **API:** https://api.virtuals.io
- **App / trading:** https://app.virtuals.io
- **Chains served include:** BASE and ROBINHOOD (as returned by the API)

VaultX deploys no contracts of its own and never holds user funds. Portfolio balances are read from public chain RPC endpoints (Base and Robinhood Chain).

## $VAULTX Token

**$VAULTX is launching on Virtuals Protocol.** The official contract address will be published here and on the official site once the token is live.

> **Scam guard:** No official $VAULTX contract address has been published yet. Anything claiming to be $VAULTX before the official announcement here is fake — always confirm the contract address on this repository and the official site before trading.

## How VaultX Fits the Token Lifecycle

```text
Virtuals Launch (app.virtuals.io)
       |
       v
   On Curve
       |
       v
   Graduated
       |
       +--> Token discovery & market views
       +--> Token detail (stats, holders, liquidity)
       +--> Trade on Virtuals (app.virtuals.io)
       +--> Portfolio valuation (VIRTUAL, estimate)

