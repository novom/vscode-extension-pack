# Novom Extension Pack

Novom Extension Pack is a project that bundles our preferred VS Code extensions for developing Javascript applications.

## Prerequisites

* [Node](https://nodejs.org) v10.15 (it is recommended to install it via [NVM](https://github.com/creationix/nvm))
* [vsce](https://github.com/Microsoft/vscode-vsce) Visual Studio Code Extensions CLI
* [Yeoman](https://yeoman.io/) 
* [generator-code](https://www.npmjs.com/package/generator-code) VS Code Extension generator for Yeoman

## How To

### Make a change to the included extensions

* Find the extension's package name located next to its display name in the VSCode Extensions Marketplace.
* Edit the `extensionPack` entries located in `package.json`.

### Bundle the extension pack

* From the project's root directory, run `vsce package`.
* Voila! A fresh `novom-extension-pack-*.*.*.vsix` file has been generated.

### Install the extension pack

* Navigate to your Visual Studio Code extension tab.
* Open the additional options menu (...) and select `Install from VSIX...`.

## Contributing

**Never** commit directly on master, instead use branches and pull requests.

Once approved, a Pull request is merged in `master` by its author. Also, it must be squashed before merging,
either manually or using GitHub's `Squash and merge` feature.

## Relevant Documentation

* [Visual Studio Code Extension API](https://code.visualstudio.com/api)