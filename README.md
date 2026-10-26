# sorai

Run your Sorai store from the shell. `sorai` lists and updates products,
prices, pages and orders, opens checkout links and reads sales analytics,
with JSON output built for scripts and AI agents.

This repository holds the releases. Download a binary from
[Releases](https://github.com/sorai-ai/cli/releases).

## Install

```sh
brew install sorai-ai/tap/sorai
curl -fsSL https://sorai.ai/install.sh | sh   # macOS and Linux, into ~/.local/bin
```

On Windows, download the zip for your CPU from the latest release.

## Use

Mint a secret key (`ssk_...`) from the API keys page of your Sorai console,
then:

```sh
export SORAI_API_KEY=ssk_...
sorai whoami
sorai products list --store my-shop --q ebook
sorai guide          # a guide for AI agents: every command and flag
```

Commands that change data take `--dry-run`, which prints what would change
and changes nothing.
