# javascript-library-template [![GitHub license](https://img.shields.io/github/license/vvo/javascript-library-template?style=flat)](https://github.com/vvo/javascript-library-template/blob/master/LICENSE) ![Tests](https://github.com/vvo/javascript-library-template/workflows/Tests/badge.svg) [![codecov](https://codecov.io/gh/vvo/javascript-library-template/branch/master/graph/badge.svg)](https://codecov.io/gh/vvo/javascript-library-template) ![npm](https://img.shields.io/npm/v/javascript-library-template)

**This JavaScript library template** allows you to easily develop, test and publish a JavaScript library with all the modern tooling you'd expect.

The main goals are:

- ease the contribution of the library by providing reproducible developer and build environements by default
- automate as much as possible, from testing to releasing

**Features:**

- [EditorConfig](https://editorconfig.org/): easy contributions from any code editor
- [ESLint](https://eslint.org/): launched in the `test` script
- [Prettier](https://prettier.io/): launched in the `test` script
- Automatic VSCode formatting and linting: using VSCode extensions recommendations and workspace settings in .`vscode/` folder
- Yarn version pinning: via [Yarn policies](https://classic.yarnpkg.com/en/docs/cli/policies/), so anyone contributing or any system accessing your library will use the same Yarn version without having to think about it
- Node.js version pinning: via [nvm](https://github.com/nvm-sh/nvm), so anyone contributing or any system accessing your library will use the same Yarn version without having to think about it
- [Jest](https://jestjs.io/): launched in the `test` script, also with the right VSCode settings providing a testing workflow inside VSCode using [`vscode-jest`](https://github.com/jest-community/vscode-jest) extension
- [GitHub actions](https://github.com/features/actions): automatic testing and releasing from GitHub: npm publish and GitHub releases are automatically created. Note that the package.json in your repository is never updated (the version is always `0.0.0-development`), only the one in npm is updated. Find more information about this in the [semantic-release documentation](https://semantic-release.gitbook.io/semantic-release/support/faq#why-is-the-package-jsons-version-not-updated-in-my-repository). This is surprising at first but actually smart and as long as you display the published version in your README (like this template does) then you're fine
- [semantic-release](https://semantic-release.gitbook.io/semantic-release/): allows for automatic releases based on semver.org and [conventional commits specification](https://www.conventionalcommits.org/). The defaults are taken from the [Angular git commit guidelines](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines)
- [Codecov](https://codecov.io/): launched in the `test` script on CI, ensures code coverage does not decreases on pull requests

## Setup

editor config
nvm
yarn
codecov
github actions

## Status

The template is still pretty new (March 2020) and was done to author JavaScript libraries using ECMAScript modules for Node.js >= 12. Gradually, or given requests, we can make update it to author libraries also for browsers with best practices. Just open an issue if you'd like to contribute.
