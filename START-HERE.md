# ArcLotls portable miner (preview)

Extract the entire archive before launching. Keep its files together.

- Windows x64: double-click **Launch ArcLotls.cmd**.
- Linux x64: run `./launch.sh` from a terminal. CI builds use Ubuntu 22.04. Local builds record their build OS and glibc in release.json; use that glibc version or newer unless separately validated.
- The launcher opens your default browser and prints a link. Open that link in your normal browser profile with MetaMask installed if necessary. Keep the launcher running.
- Connect MetaMask, check the chain, contract, recipient, and mint price, choose an engine, then Start mining. Every mint requires your confirmation and its displayed payment plus gas.
- Stop prevents new signature requests. Dismiss any prompt already open in MetaMask. Submitted transactions remain tracked.
- Close the launcher with Ctrl+C when finished. For testnet, launch with `--testnet`. For terminal-only startup, add `--no-open`.

No Node.js, pnpm, CUDA toolkit, or compiler installation is required. NVIDIA CUDA needs a compatible installed NVIDIA driver. Other GPU engines depend on your browser and graphics driver; see COMPATIBILITY.md. Use an up-to-date Chromium-based browser with MetaMask; GPU detection and startup checks determine availability.

Auto tries CUDA, then WebGPU, then one CPU worker. CPU uses verified WASM when available and JavaScript otherwise. Explicit engine selections do not silently switch to a different engine. Initialization fallback reasons appear beside the engine selector. A runtime failure pauses mining: choose an engine and Start again, or restart the launcher after a CUDA worker failure. No GPU availability or profitability is promised.

Mainnet is the default. The miner checks wallet network/account, simulates transactions, and verifies mining proofs; it does not audit the deployment or its authority wallets. Connection settings are in config.mainnet.json and config.testnet.json; change RPC or CUDA device index there if needed. Never put private keys or seed phrases in those files. Keep the default port 18732: transaction recovery belongs to the browser profile and local origin, so changing the port or profile creates separate history. If the port is occupied, close the other miner; the launcher never silently switches ports.

Pending transactions are reconciled before mining resumes. If a signature outcome is unknown, inspect MetaMask Activity and use the existing recovery control. Do not clear browser storage to bypass an unresolved transaction.

The service listens only on 127.0.0.1 and authorizes its API using the token in the launch link. Treat that link as local session access. Wallet signing stays in MetaMask; the local service accepts no wallet keys. Do not expose the service as a public or remote worker.

Download the platform archive and its .sha256 file from the same release. Verify the archive checksum before extracting. The app checks packaged assets at startup; checksums detect corruption but are not publisher signatures. This preview is not code-signed. Updates are manual: stop the old launcher and extract a new version; keep the same browser profile and port for transaction recovery.

NODE-LICENSE.txt, THIRD-PARTY-NOTICES.txt, and CUDA-LICENSE.txt (when CUDA is included) contain redistribution notices. Linux CUDA bundles also include GNU runtime notices and the GPL text with the runtime exception in the notices. release.json lists the version, platform requirements, bundled runtime, and dependencies.
