# MintShot Themes

MintShot Themes is an open-source collection of dark and light VS Code themes with refined neutral surfaces, distinct accent palettes, soft contrast, and bright syntax highlighting designed for long coding sessions.

MintShot Themes is from the company Mint Shot.

Website: https://mintshot.app

GitHub repo: https://github.com/timfewi/mintshot-theme

## Install

### From the VS Code Marketplace

Search for `MintShot Themes` in the Extensions view and install it like any other VS Code extension.

### From a `.vsix` file

1. Download the latest `.vsix` from the GitHub repo or a release.
2. In VS Code, run `Extensions: Install from VSIX...`.
3. Select the downloaded file.
4. Open `Preferences: Color Theme` and choose a MintShot theme.

## Included themes

- `MintShot Dark`
- `MintShot Dark Blue`
- `MintShot Dark Orange`
- `MintShot Dark Purple`
- `MintShot Dark Red`
- `MintShot Dark Yellow`
- `MintShot Dark Green`
- `MintShot Dark VS2019`
- `MintShot Dark VS2019 Dimmed`
- `MintShot Light`
- `MintShot Light Blue`
- `MintShot Light Gray`
- `MintShot Light Gold`
- `MintShot Light Rose`
- `MintShot Light Lavender`
- `MintShot Light Sand`
- `MintShot Light White`

## Work on the theme locally

If you want to help improve the project, you can work on it locally in a standard VS Code extension workflow.

1. Clone the repo:

   ```bash
   git clone https://github.com/timfewi/mintshot-theme.git
   cd mintshot-theme
   ```

2. Open the repo in VS Code.
3. Press `F5` to launch an Extension Development Host.
4. In the new window, open `Preferences: Color Theme`.
5. Select one of the MintShot themes and verify your changes live.

## Where to make changes

- `themes/` contains the theme JSON files.
- `package.json` contains extension metadata plus packaging and publishing scripts.
- `assets/` contains branding assets such as the extension icon.
- `.github/workflows/publish.yml` contains the GitHub Actions packaging and publishing workflow.

## Packaging

To create a local `.vsix` package:

```bash
bun run package
```

This builds a `.vsix` you can install manually or attach to a GitHub release.

## Contributing

Contributions are welcome.

If you want to collaborate:

- open an issue for bugs, theme tweaks, or new theme ideas
- submit a pull request with your changes
- share screenshots if your change affects colors or readability

Repo: https://github.com/timfewi/mintshot-theme

## Publishing

This project publishes to the VS Code Marketplace.

### Manual publish

```bash
bun run publish:vsce
```

### GitHub Actions publish

The workflow in `.github/workflows/publish.yml` packages the extension on version tags and publishes it when the `VSCE_PAT` repository secret is configured.

## License

MintShot Themes is released under the MIT License.
