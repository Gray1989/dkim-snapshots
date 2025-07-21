# DKIM Snapshots 📬🔐

This repository retains DNS records—specifically [DKIM (DomainKeys Identified Mail)](https://en.wikipedia.org/wiki/DomainKeys_Identified_Mail) TXT records—for personal archival purposes. It archives snapshots of public DKIM keys for a selected set of domain–selector pairs.

Although this repo was created for personal reference, it is publicly available for anyone to explore, fork, or use however they like. ✅

## 🏗️ How It Works

- A GitHub Actions workflow is run manually
- DKIM selectors are listed in `selectors.txt` (as `domain:selector`)
- Each key is retrieved using `dig` and stored in a file under [`results/`](./results)
- Changes are committed by the snapshot bot and pushed to the repository
- Snapshots are bundled, attested, and uploaded to [GitHub Releases](https://github.com/Gray1989/dkim-snapshots/releases)

## 📜 License

This repository is dedicated to the public domain under the [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) license.

> You are free to copy, modify, distribute, and use this repository and its contents for any purpose, without restriction.
