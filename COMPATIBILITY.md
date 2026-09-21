# Compatibility

This is an unsigned prerelease for Windows x64 and Linux x64. Linux requires glibc 2.35 or newer. Install a compatible graphics driver and a browser with MetaMask.

| Engine | Intended hardware | Validation limits |
| --- | --- | --- |
| CUDA | NVIDIA RTX 30-, 40-, and 50-series (sm_86, sm_89, sm_120) | RTX 50-series proof checks have passed on Windows and Linux/WSL2; RTX 30/40 physical validation is pending |
| WebGPU | Browser-exposed NVIDIA, AMD, or Intel adapter | NVIDIA checks have passed on Windows; AMD/Intel and physical Linux coverage are pending |
| CPU | Windows/Linux x64 | WASM SIMD checks have passed on both platforms; JavaScript fallback is available |

Software GPU adapters can fail startup responsiveness calibration. Auto then tries CPU; explicit engine selections report their failure. Compiling for an architecture does not certify that hardware. WSL2 testing does not certify every Linux desktop. These are compatibility checks, not sustained performance or profitability claims.

Mac, ARM, remote workers, unattended signing, installers, and automatic updates are outside this release. Keep the release marked prerelease while broader physical-hardware and pristine-machine checks remain pending.
