# VaultX

<p align="center"><strong>Every curve token, behind one door.</strong></p>

<p align="center">
  Live board and trading front-end for Pons bonding-curve tokens on Robinhood Chain.
  <br>
  🌐 Live site: <a href="https://vaultx-2.vercel.app">vaultx-2.vercel.app</a>
  &nbsp;·&nbsp;
  𝕏 <a href="https://x.com/VaultX">x.com/VaultX</a>
</p>

---

## What it is

VaultX is a discovery and trading front-end for bonding-curve tokens launched on
[Pons](https://ponsfamily.com) (Robinhood Chain, chain ID 4663). All data is read
live from the chain — no demo data, no mock prices.

- **Live board** — every Pons launch, with price, market cap, 24h volume, curve
  reserve and graduation progress. Sort by newest, oldest, market cap, volume or
  curve progress; filter by On curve / Graduating / Surfaced.
- **Trade the curve** — buy and sell directly against the bonding curve at its
  constant-product price, including the curve's real 3.8% input fee. No VaultX
  markup.
- **Graduation tracking** — a token graduates at 4.2 ETH real reserve, then keeps
  trading on its Uniswap pool (linked via DexScreener).
- **Swap** — a dedicated swap view with a searchable token picker, using the same
  live token list and the same quoting as the detail view.
- **Launchpads** — Pons at a glance: live launch stats and the same token grid.
- **Portfolio** — connect a wallet and see the curve tokens it actually holds,
  valued at live curve prices (ETH + USD), with a total-value summary.
- **Docs** — how the curve works, the 3.8% fee, graduation, and the risks.
- **$VAULTX** — coming soon. The token is **not launched**: there is no contract
  address, no price, and nowhere to buy it yet. Anything claiming to be $VAULTX
  before the official announcement is fake.

## Tech

- Single self-contained `index.html` — no build step, no backend.
- Reads live from the Pons V2 factory (`0x7ed5…ec7e`) on Robinhood Chain.
- Three RPC endpoints with automatic failover and a stale-data banner, so one
  failing endpoint never blanks the board.
- Token images come from each token contract's `logo()` function, with four IPFS
  gateway fallbacks.
- Wallet via EIP-1193 (injected wallets). Trading is real on-chain transactions —
  always test with a small amount first.

## Run it

```bash
# Option 1: open the file directly
open index.html

# Option 2: serve it locally
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy

**GitHub Pages** (free, recommended):

1. Push this repo to GitHub.
2. Settings → Pages → Source: *Deploy from a branch* → Branch: `main` → Save.
3. Your site is live at `https://vaultx-apps.github.io/vaultx/`.

**Vercel:** import the repo, or drag `index.html` into a project as a single
file (it must be named `index.html` at the project root).

## Structure

```
.
├── index.html            # The whole site — board, Swap, Launchpads, Portfolio, Docs
├── LICENSE
└── README.md
```

## Disclaimer

VaultX is a front-end. Bonding-curve tokens are extremely volatile and many go
to zero — do your own research. VaultX charges no fee and never holds your funds;
trades are signed by your own wallet.

## License

MIT — see [LICENSE](LICENSE).
