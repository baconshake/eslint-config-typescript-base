# @baconshake/eslint-config-typescript-base

This package provides Baconshakes's .eslintrc as an extensible shared config.

## Installation

For some reason, it's not sufficient to run `npx install-peerdeps --dev @baconshake/eslint-config-typescript-base`,
so you either have to install the `peerDependencies` manually:

```sh
npm info "@baconshake/eslint-config-typescript-base" peerDependencies
```

Or run this script:

```sh
(
  export PKG="@baconshake/eslint-config-typescript-base";
  npm info "$PKG@latest" peerDependencies --json | command sed 's/[\{\},]//g ; s/: /@/g' | xargs npm install --save-dev "$PKG@latest"
)
```

## Usage

In you `.eslintrc`, simply extend the config.

```json
{
  "extends": ["@baconshake/eslint-config-typescript-base"]
}
```
