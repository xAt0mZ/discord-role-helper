# Installation

Clone the repo
```sh
yarn dev
```
You're up and running !


# Project creation steps - for history

## References
* [Yarn 2 migration guide](https://yarnpkg.com/getting-started/migration)
* [Vite quickstart](https://vitejs.dev/guide/#scaffolding-your-first-vite-project)
* [Yarn sdk](https://yarnpkg.com/getting-started/editor-sdks)

## FS and project creation
```sh
yarn create vite client --template react-ts
cd client
yarn set version stable
```
remove `nodeLinker: node_modules` from `.yarnrc.yml`
```sh
yarn install
rmdir node_modules
```

## Add some yarn sdks/plugins
* `yarn plugin import interactive-tools` > Enable `yarn upgrade-interactive` | [Link](https://yarnpkg.com/cli/upgrade-interactive)
* `yarn plugin import typescript` > Enable auto adding devDependency `@types/XXX` when adding `XXX` dependency | [Link](https://yarnpkg.com/api/modules/plugin_typescript.html)
* yarn plugin import version
* yarn plugin import workspace-tools
* `yarn dlx @yarnpkg/sdks vscode` > Enable VSCode SDK | [Link](https://yarnpkg.com/getting-started/editor-sdks#vscode)

## Configure VSCode
* `Ctrl+Shift+P > Typescript: Select typescript version > Use workspace version` > resolve the types & co in VSCode
* Install [ZipFS](https://marketplace.visualstudio.com/items?itemName=arcanis.vscode-zipfs) > enable `Ctrl+Click (Go To Definition)` in `.ts/.tsx` files


`Vite + React TS + Yarn Berry with PnP` project is enabled