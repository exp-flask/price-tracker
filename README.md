##From Scratch
New Next.js project:
```npx create-next-app@latest```



##Node Version and fnm
There are a couple node version managers out there like `nvm` and `fnm`. This project uses the Rust based `fnm`, which focuses on project dir scope rather than globally like nvm.

###Setting up fnm on this local project
If not already installed, install via package manager: `choco install fnm` (Windows) or `brew install fnm` (macOS)

Set desired node version in a new .node-version file: 
```echo "v21.7.2" > .node-version```
(optional) peruse available versions `fnm list-remote` and `fnm install [version]` if your not sure

auto-switch to node version via fnm when navigating to directory:
Windows (PowerShell)
```fnm env --use-on-cd | Out-String | Invoke-Expression```
macOS (zsh)
```eval "$(fnm env --use-on-cd)"```
If version not already installed, answer `y` to prompt

Check versions were updated with `fnm current`, `node -v`, `npm -v`