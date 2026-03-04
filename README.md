<p align="center">
  <img src="https://raw.githubusercontent.com/mcp-tool-shop-org/brand/main/logos/escape-the-valley/readme.png" width="400" alt="Ledger Trail: Escape the Valley">
</p>

<p align="center">
  <a href="https://www.npmjs.com/package/@mcptoolshop/escape-the-valley"><img src="https://img.shields.io/npm/v/@mcptoolshop/escape-the-valley" alt="npm"></a>
  <a href="https://pypi.org/project/escape-the-valley/"><img src="https://img.shields.io/pypi/v/escape-the-valley" alt="PyPI"></a>
  <img src="https://img.shields.io/badge/license-MIT-blue" alt="MIT License">
</p>

<p align="center">
  <em>A survival game where the trail is the teacher and the ledger keeps you honest.</em>
</p>

---

## Install

```bash
npx @mcptoolshop/escape-the-valley tui --seed 42
```

Or install globally:

```bash
npm install -g @mcptoolshop/escape-the-valley
trail tui --seed 42
```

Also available via pip:

```bash
pip install escape-the-valley
trail tui --seed 42
```

## What Is This?

Escape the Valley is an Oregon Trail-style survival game that runs in your terminal. Lead a party of settlers through a procedurally generated wilderness. Manage food, water, wagon condition, and morale while navigating events, hazards, and hard choices.

An optional AI Game Master (powered by Ollama) narrates your journey with three distinct storytelling voices. An optional XRPL Testnet ledger backpack tracks your supply changes as on-chain receipts.

## How It Works

This npm package downloads a pre-built binary from GitHub Releases with SHA256 verification. No Python installation required.

- Binaries cached at `~/.cache/mcptoolshop/escape-the-valley/`
- `--clear-cache` to remove cached binaries
- `--print-cache-path` to show cache location

## Links

- [Source code](https://github.com/mcp-tool-shop-org/escape-the-valley)
- [PyPI package](https://pypi.org/project/escape-the-valley/)
- [Landing page](https://mcp-tool-shop-org.github.io/escape-the-valley/)

## License

MIT

Built by <a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a>
