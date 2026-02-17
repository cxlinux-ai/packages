# CX Linux APT Repository

Official package repository for CX Linux.

## Quick Install

```bash
# Add GPG key
curl -fsSL https://repo.cxlinux.ai/key.gpg | sudo gpg --dearmor -o /etc/apt/keyrings/cxlinux.gpg

# Add repository
echo "deb [signed-by=/etc/apt/keyrings/cxlinux.gpg] https://repo.cxlinux.ai/apt stable main" | sudo tee /etc/apt/sources.list.d/cxlinux.list

# Install
sudo apt update
sudo apt install cx-terminal
```

## Available Packages

- `cx-terminal` - CX Terminal emulator
- `cx-terminal-nightly` - Nightly builds
- `cx-core` - Core CX Linux components

## Verify GPG Key

```bash
curl -fsSL https://repo.cxlinux.ai/key.gpg | gpg --show-keys
```

Fingerprint: `98E4 FB1D C6AE 2D81 403B 35B6 760F C68E EBB7 D6E9`
