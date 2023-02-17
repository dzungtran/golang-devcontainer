# Golang devcontainer

A template devcontainer to work with multiple Golang repositories in a devcontainer.
For lazy deverlopers who work with multiple GO projects and don't want switch go version on local.

Any feedback and pull requests are welcome and highly appreciated. Feel free to open issues just for comments and discussions.

## Requirements
    
- Docker (ofcouse)
- IDE supports devcontainer
- Minimum GO version: 1.18 - (uses `go work` feature)

## Usages

> Click **[Use this template](https://github.com/dzungtran/golang-devcontainer/generate)** feature for personal use. And **Fork** when you want contribute this repo.

- Clone this repo to your local.
- Open VSCode with cloned folder.
- In VS Code: press `Cmd + shift + P` or `Win + shift + P` to open `Command Palette` popup.
- Search `Dev containers: Open Folder in Container`, then choose current folder.
- Waiting to initial container success.
- Open VSCode terminal, cd to folder `src`, clone your Golang repos in this.
- Back to root folder, run command `go work use ./src/<your-golang-repo-folder-name>`.
- Enjoy.

## Notes

- Maybe you need add you ssh key to this container for project cloning.
- You can click **[Use this template](https://github.com/dzungtran/golang-devcontainer/generate)** to customize your devcontainer and personal use.
- In case you're working on private repos: you will need add `export GOPRIVATE=github.com/<git-user>/*` to `~/.bashrc`
- You can change default GO version of container by: edit file `devcontainer.json`, default this repo support GO version 1.19.
```
"image": "mcr.microsoft.com/vscode/devcontainers/go:0-1.19",
```