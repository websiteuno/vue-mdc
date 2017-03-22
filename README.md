<p align="center">
  <img src="logo.svg"/>
  <br/>
  <a href="https://circleci.com/gh/posva/vue-mdl">
    <img alt="Circle CI" src="https://img.shields.io/circleci/project/posva/vue-mdl/develop.svg" />
  </a>
  <a href="https://codecov.io/gh/posva/vue-mdl">
    <img alt="Codecov Coverage" src="https://img.shields.io/codecov/c/github/posva/vue-mdl/develop.svg?maxAge=2592000" />
  </a>
  <br>
  <a href="https://david-dm.org/posva/vue-mdl#info=devDependencies" title="devDependency status"><img src="https://david-dm.org/posva/vue-mdl/dev-status.svg"/></a>
  <a href="https://david-dm.org/posva/vue-mdl#info=peerDependencies" title="peerDependency status"><img src="https://david-dm.org/posva/vue-mdl/peer-status.svg"/></a>
  <br>
  <a href="https://www.npmjs.com/package/vue-mdl"><img src="https://img.shields.io/npm/v/vue-mdl.svg" alt="Latest npm release"></a>
  <a href="https://gitter.im/posva/vue-mdl?utm_source=badge&utm_medium=badge&utm_campaign=pr-badgel"><img src="https://badges.gitter.im/posva/vue-mdl.svg" alt="Gitter"></a>
</p>
[![npm](https://img.shields.io/npm/v/vue-mdc.svg)](https://www.npmjs.com/package/vue-mdc) [![vue2](https://img.shields.io/badge/vue-2.x-brightgreen.svg)](https://vuejs.org/)

# VueMdc

> Material Components Web for Vue.js

## Installation

```bash
npm install --save vue-mdc
yarn install -D vue-mdc
```

## Usage

### Bundler (Webpack, Rollup)

```js
import Vue from 'vue'
import VueMdc from 'vue-mdc'
// You need a specific loader for CSS files like https://github.com/webpack/css-loader
import 'vue-mdc/dist/vue-mdc.css'

Vue.use(VueMdc)
```

### Browser

```html
<!-- Include after Vue -->
<!-- Local files -->
<link rel="stylesheet" href="vue-mdc/dist/vue-mdc.css"></link>
<script src="vue-mdc/dist/vue-mdc.js"></script>

<!-- From CDN -->
<link rel="stylesheet" href="https://unpkg.com/vue-mdc/dist/vue-mdc.css"></link>
<script src="https://unpkg.com/vue-mdc"></script>
```

### Docs

WIP 😁

## Development

### Launch visual tests

```bash
npm run dev
```

### Launch Karma with coverage

```bash
npm run dev:coverage
```

### Build

Bundle the js and css of to the `dist` folder:

```bash
npm run build
```


## Publishing

The `prepublish` hook will ensure dist files are created before publishing. This
way you don't need to commit them in your repository.

```bash
# Bump the version first
# It'll also commit it and create a tag
npm version
# Push the bumped package and tags
git push --follow-tags
# Ship it 🚀
npm publish
```

## License

[MIT](http://opensource.org/licenses/MIT)
