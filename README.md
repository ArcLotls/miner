# ArcLotls miner

Portable ArcLotls miner downloads for Windows x64 and Linux x64, with CUDA, WebGPU, and CPU engines. Wallet signing stays in your browser with MetaMask; every mint requires confirmation.

Download the platform archive and matching SHA-256 file from [Releases](https://github.com/ArcLotls/miner/releases). Preview versions are marked prerelease. Follow [START-HERE.md](START-HERE.md) and check [COMPATIBILITY.md](COMPATIBILITY.md) before running.

No Node.js, pnpm, compiler, or CUDA toolkit installation is required. You provide a compatible graphics driver and a browser with MetaMask. The miner defaults to Arc mainnet and native USDC payment; mint payments and gas are separate from any mining rewards.

This repository hosts public guides, downloadable release assets, and issue reports. The application source repository is private. Downloads include readable bundled application code and required dependency notices.

The miner is free to use, including for mining for profit. You may share unchanged official bundles with their notices and a copy of the [license terms](LICENSE.md). The four Markdown guides are licensed under CC BY 4.0; third-party components retain their own licenses. See [LICENSE.md](LICENSE.md) for the full scope and conditions.

The preview is unsigned. Checksums detect changed bytes but do not authenticate the publisher. Hardware coverage is limited; no mining speed or profitability is guaranteed. The miner checks wallet account/network, simulates transactions, and verifies proofs, but does not perform a deployment-wide audit.

For support, open an issue with your operating system, browser, selected engine, and a redacted error message. Never post private keys, seed phrases, the token-bearing localhost launch link, or unredacted logs containing personal paths. Avoid posting wallet addresses unless you intend to make them public.
