# DXVK4AndroidBuilds 🚀

GitHub Actions-based build repository for DXVK GPLAsync.

This repository packages DXVK GPLAsync source code for two targets:

- `x64` 🖥️
- `ARM64EC` ⚙️

The resulting packages are prepared as `WCP` archives and published as GitHub Releases 📦

## What It Does 🛠️

This workflow:

1. Clones the DXVK GPLAsync repository.
2. Applies the relevant patch set.
3. Builds `x64` and `ARM64EC` outputs.
4. Archives the packages as `.wcp` files.
5. Publishes the results as artifacts and releases.

## Usage ▶️

The workflow is triggered manually:

- Open the repository on GitHub.
- Go to the **Actions** tab.
- Select `Build DXVK GPLAsync WCP`.
- Click **Run workflow**.

Optional inputs:

- `repo_url`: DXVK GPLAsync repository to build
- `ref`: Branch, tag, or commit

Default repository:

- `https://gitlab.com/Ph42oN/dxvk-gplasync.git`

## Outputs 📤

After a successful run, you will get:

- `dxvk-gplasync-<version>-x86_64.wcp`
- `dxvk-gplasync-<version>-arm64ec.wcp`

The files are uploaded as artifacts first and then published under the GitHub Release.

## Release Naming 🏷️

The release tag is created in the following format:

- `dxvk-gplasync-<version>`

## Requirements ✅

No local setup is required. The entire build runs on GitHub Actions.

## License 📄

This repository is subject to the license terms stated in the `LICENSE` file.
