# ArcLotls miner

Portable ArcLotls miner downloads for Windows x64 and Linux x64, with CUDA, WebGPU, and CPU engines. Wallet signing stays in your browser with MetaMask; every mint requires confirmation.

**Unsigned prerelease · 0.1.0-preview.2**

- [Windows x64 download](https://github.com/ArcLotls/miner/releases/download/miner-v0.1.0-preview.2/arclotls-miner-0.1.0-preview.2-windows-x64.zip) · [SHA-256 checksum](https://github.com/ArcLotls/miner/releases/download/miner-v0.1.0-preview.2/arclotls-miner-0.1.0-preview.2-windows-x64.zip.sha256)
- [Linux x64 download](https://github.com/ArcLotls/miner/releases/download/miner-v0.1.0-preview.2/arclotls-miner-0.1.0-preview.2-linux-x64.tar.gz) · [SHA-256 checksum](https://github.com/ArcLotls/miner/releases/download/miner-v0.1.0-preview.2/arclotls-miner-0.1.0-preview.2-linux-x64.tar.gz.sha256)
- [Getting started](START-HERE.md) · [Compatibility and hardware limitations](COMPATIBILITY.md) · [All releases](https://github.com/ArcLotls/miner/releases)

Check compatibility and verify the archive checksum before extracting and running. Broader hardware validation remains pending.

No Node.js, pnpm, compiler, or CUDA toolkit installation is required. You provide a compatible graphics driver and a browser with MetaMask. The miner defaults to Arc mainnet and native USDC payment; mint payments and gas are separate from any mining rewards.

This repository hosts public guides, downloadable release assets, and issue reports. The application source repository is private. Downloads include readable bundled application code and required dependency notices.

The miner is free to use, including for mining for profit. You may share unchanged official bundles with their notices and a copy of the [license terms](LICENSE.md). The four Markdown guides are licensed under CC BY 4.0; third-party components retain their own licenses. See [LICENSE.md](LICENSE.md) for the full scope and conditions.

The preview is unsigned. Checksums detect changed bytes but do not authenticate the publisher. Hardware coverage is limited; no mining speed or profitability is guaranteed. The miner checks wallet account/network, simulates transactions, and verifies proofs, but does not perform a deployment-wide audit.

For support, open an issue with your operating system, browser, selected engine, and a redacted error message. Never post private keys, seed phrases, the token-bearing localhost launch link, or unredacted logs containing personal paths. Avoid posting wallet addresses unless you intend to make them public.
