# Go Dev Container

A complete development container for Go for use with VSCode/GitHub Codespaces

---

## Features

 - Go with basic Go development tools
 - Uses my [dotfiles](https://github.com/willfantom/.files) via a devcontainer feature
 - Use on `amd64` and `aarch64`

## Local Usage Requirements

- [Docker](https://www.docker.com/products/docker-desktop) installed and running
- [VS code](https://code.visualstudio.com/download) installed
- [VS code remote containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) installed

## Usage

 1. In the root of your project, create a directory named `.devcontainer`
 2. Copy the `devcontainer.json` file from this repository to the newly created directory
 3. Open the project in the devcontainer via the [devcontainer CLI](https://github.com/devcontainers/cli), the commands in VSCode, or in a GitHub Codespace

## Image Customization

You can use this image along with devcontainer features, for example my [dotfiles](https://github.com/willfantom/.files) can be included by adding the following snippet in the `devcontainer.json` files:
```json
"features": {
  "ghcr.io/willfantom/features/dotfiles:1": {}
},
```
Docker-In-Docker and Docker-Outside-Of-Docker can also be used along with this devcontainer:
  - `"ghcr.io/devcontainers/features/docker-in-docker:2": {}`
  - `"ghcr.io/devcontainers/features/docker-outside-of-docker:1": {}`
