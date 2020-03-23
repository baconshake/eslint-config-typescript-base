# @baconshake/eslint-config-typescript-base

This package provides Baconshakes's .eslintrc as an extensible shared config.

It's built upon [`eslint-config-airbnb-base`](https://www.npmjs.com/package/eslint-config-airbnb-base)

## Installation

This package has a few peer dependencies. You can install them a few different ways:

```sh
npx install-peerdeps @baconshake/eslint-config-typescript-base
```

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
