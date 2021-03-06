<!-- ![Logo of the project](./images/logo.sample.png) -->

# devise

> Make great game documentation

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/de76c263ff0941f1894d4e76565b99bf)](https://www.codacy.com/app/multi-cell/devise-ante?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=multi-cell/devise-ante&amp;utm_campaign=Badge_Grade)
[![Known Vulnerabilities](https://snyk.io/test/github/multi-cell/devise-ante/badge.svg)](https://snyk.io/test/github/multi-cell/devise-ante)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fmulti-cell%2Fdevise-ante.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fmulti-cell%2Fdevise-ante?ref=badge_shield)
[![Greenkeeper badge](https://badges.greenkeeper.io/multi-cell/devise-ante.svg)](https://greenkeeper.io/)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com)

Devise is a web application for making easily-searchable, presentable, modular game documentation.

## Installing / Getting Started

Currently, there isn't a way to just install the app to use in production, but we'll get there (I promise!).

## Developing

### Contributing

Please note that this project is released with a [Contributor Code of Conduct](.github/CODE-OF-CONDUCT.md). By participating in this project you agree to abide by its terms.

### Built With

Devise relies on the following technologies:

+ Vue
+ Vuex
+ GraphQL/Graphcool
+ Apollo
+ AT-UI

### Prerequisites
You'll need two things:

+ [Node Current](https://nodejs.org/en/)
+ A [Graphcool](https://www.graph.cool/) account


### Setting up Dev

Here's a brief intro about what a developer must do in order to start developing
the project further:

```shell
# Download the project
git clone https://github.com/multi-cell/devise.git
cd devise/

# Install dependencies with a package manager of your choice
npm install
# OR
yarn
```

That should be everything you need to get up and running for development.

### Building

Building the application is pretty simple:

```shell
# Build and launch server for development
npm run dev

# Or, build for production
npm run build
```

Devise is built using webpack, and has different options for development and production.

#### Development

We use webpack-dev-server for hot-module replacement. While it's up and running, you also have access to the following cool tools:

+ [webpack-dashboard](https://github.com/FormidableLabs/electron-webpack-dashboard). Install the desktop app and see the magic!
+ [Friendly webpack errors](https://www.npmjs.com/package/friendly-errors-webpack-plugin). Actually understand what the problem is!
+ Desktop notifications, for when your build fails.

#### Production

When building for production, we'll minify the code and such. It's not too special. You'll find the output in the `dist` directory.

## Versioning

We use [SemVer](http://semver.org/) for versioning. Or, we will, when we get to that point.

## Configuration

More info to come.

## Tests

We rely mainly on integration testing to make sure things work properly, using [Cypress](https://cypress.io). Check those docs when you need to write tests. Any written specs are run automatically during CI, and are fully recorded in order to review any issues that arise.

If you want to run tests, it's pretty simple.
```sh
# Build production version
npm run build
# Launch test server
npm run test:integration
```

This launches a script that instantiates a [serve](https://github.com/zeit/serve) instance in the `dist` folder, runs the tests, then kills the server. This process will change with the introduction of a GraphQL server in the near future.

## Style guide

[![JavaScript Style Guide](https://cdn.rawgit.com/standard/standard/master/badge.svg)](https://github.com/standard/standard)

That badge really says it all. You don't really need to worry about running formatting or linting commands; when you stage files and make a commit,
`lint-staged` will make sure to lint your files and format them using `prettier-standard`. But, if you must know:

```shell
# Lint JS files
npm run test:lint

# Format JS files in src/
npm run test:format
```

## API Reference

The API for devise is found in another castle, which is still being built. Updates to come!

## Database

Currently, the database that this project uses is provided by Graphcool. We'll have instructions in the near future.

## Licensing

This project is licensed under the Apache 2.0 license, which you can check out in the [LICENSE](LICENSE) file.

---

[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fmulti-cell%2Fdevise-ante.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fmulti-cell%2Fdevise-ante?ref=badge_large)
