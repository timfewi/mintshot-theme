# MintShot

MintShot is a dark VS Code theme with mint-forward accents, low-glare backgrounds, and bright syntax contrast for long coding sessions.

## Installation

Once the extension is published, install it from:

- the VS Code Marketplace by searching for `MintShot`

You can also install it manually from a release artifact:

1. Download the latest `.vsix` from the repo's releases.
2. In VS Code, run `Extensions: Install from VSIX...`.
3. Select the downloaded file and switch your color theme to `MintShot`.

## Local development

To work on the theme locally:

1. Open this repo in VS Code.
2. Press `F5` to launch an Extension Development Host.
3. In the new window, open `Preferences: Color Theme` and select `MintShot`.

To build a local package:

```bash
npm run package
```

That command creates a `.vsix` you can install locally or attach to a GitHub release.

## Publishing

This repo is set up for the VS Code Marketplace.

- `npm run publish:vsce` publishes to the VS Code Marketplace.

The included GitHub Actions workflow can also package the extension and publish it when the required secrets are configured.

- `VSCE_PAT` for the VS Code Marketplace publisher token

## Repository layout

- `package.json` contains extension metadata and publishing scripts.
- `themes/mintshot-dark-color-theme.json` contains the actual theme definition.
- `.github/workflows/publish.yml` packages and publishes release builds.
