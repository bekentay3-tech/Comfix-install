# Comfix

Comfix is a free Windows desktop app for working with a local portable ComfyUI installation.

It is made for users who want to quickly install ComfyUI, launch it, update it, check installed nodes and models, and analyze a workflow project before running it.

## Download

[Download the latest version](https://github.com/bekentay3-tech/Comfix-install/releases/latest) - the `Comfix_..._x64-setup.exe` file under Assets.

## Features

- install a portable ComfyUI build;
- start and stop ComfyUI from the app;
- check for and install ComfyUI and ComfyUI-Manager updates;
- browse installed custom nodes;
- browse models in the `models` folder;
- workflow JSON audit: Comfix shows which nodes and models are already available locally and which are missing;
- install the missing nodes it finds;
- save useful nodes to favorites.

## Requirements

- Windows 10 or Windows 11 x64;
- an internet connection to install ComfyUI and download Python, dependencies, nodes and models;
- Git, if you use the features that install or update repositories;
- enough free disk space for ComfyUI, models and dependencies.

## How to install

1. Download the `Comfix_..._x64-setup.exe` installer from the link above.

2. Run the installer.

3. Follow the installer steps. Comfix installs for the current user and does not need to be installed for all Windows users.

4. After installation, start Comfix from the Start menu or from the shortcut, if the installer created one.

## Updates

When a new version is released, Comfix shows a bar at the top saying "A new version of Comfix is available" with an "Update" button. The app downloads the update, installs it and restarts.

## Windows SmartScreen warning

The Comfix installer is not digitally signed yet.

Because of this, Windows may show a warning:

- `Unknown publisher`;
- `Windows protected your PC`;
- `This app is from an unknown publisher`.

This does not mean the app is paid or broken. It only means the installer is not signed with a commercial code signing certificate.

If you trust the source, click `More info` -> `Run anyway`.

## Working with ComfyUI

Comfix is not ComfyUI and does not replace it. It manages a local ComfyUI installation:

- creates the portable folder structure;
- runs the ComfyUI `.bat` file;
- checks the local `custom_nodes` and `models` folders;
- reads workflow JSON and compares it with local nodes and models;
- calls Git/Python/pip to install and update components.

It is recommended to stop ComfyUI before installing, updating or removing nodes.

## App data

Comfix keeps its settings, cache and logs in the `ComfixData` folder next to the installed app.

You can see the data path in the app under `Settings`.

## Bugs and questions

Found a bug? Report it in the [Issues](https://github.com/bekentay3-tech/Comfix-install/issues) tab.

## License

Comfix is distributed free of charge as freeware.

The source code is closed and is not distributed. You may install and use Comfix for free. You may not sell Comfix, present it as your own product, modify it, decompile it, or distribute modified versions without the author's permission.

The full terms are in [LICENSE.txt](LICENSE.txt).
