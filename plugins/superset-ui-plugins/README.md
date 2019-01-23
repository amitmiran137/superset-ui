# @superset-ui

[![Codecov branch](https://img.shields.io/codecov/c/github/apache-superset/superset-ui-legacy/master.svg?style=flat-square)](http://codecov.io/github/apache-superset/superset-ui-legacy/coverage.svg?branch=master)
[![Build Status](https://img.shields.io/travis/com/apache-superset/superset-ui-legacy/master.svg?style=flat-square
)](https://travis-ci.com/apache-superset/superset-ui-legacy)
[![David](https://img.shields.io/david/dev/apache-superset/superset-ui-legacy.svg?style=flat-square)](https://david-dm.org/apache-superset/superset-ui-legacy?type=dev)

Collection of charts that are extracted from classic [Apache Superset](https://github.com/apache/incubator-superset) and converted into plugins.

## Packages

| Package | Version |
|--|--|
| [@superset-ui/chart](https://github.com/apache-superset/superset-ui-legacy/tree/master/packages/superset-ui-chart) | [![Version](https://img.shields.io/npm/v/@superset-ui/chart.svg?style=flat-square)](https://img.shields.io/npm/v/@superset-ui/chart.svg?style=flat-square) |

#### Coming :soon:

- Data providers
- Embeddable charts
- Chart collections

### Development

[lerna](https://github.com/lerna/lerna/) is used to manage versions and dependencies between
packages in this monorepo.

```
superset-ui/
  lerna.json
  package.json
  ...
  packages/
    package1/
      package.json
      ...
      src/
      test/
      ...
      lib/
      esm/
      ...
    ...
```

### Installation

1. clone this repo
2. have yarn install package dependencies and manage the symlinking between packages for you

```sh
git clone ...superset-ui && cd superset-ui
yarn install
```

### Builds, linting, and testing

Each package defines its own build config, linting, and testing. You can have lerna run commands
across all packages using the syntax `yarn run test` (or `yarn run test:watch` for watch mode) from the root `@superset-ui` directory.

### Publishing

**Prerequisite:** You'll need an [npmjs.com](https://npmjs.com) account that is part of the `superset-ui` organization.

1. Make sure you're logged in to NPM from your shell. Run `npm login` if necessary.
2. To make the release, run `yarn run release` and follow the prompts.

### License

Apache-2.0