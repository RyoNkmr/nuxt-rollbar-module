# nuxt-rollbar-module

[![npm (scoped with tag)](https://img.shields.io/npm/v/nuxt-rollbar-module/latest.svg?style=flat-square)](https://npmjs.com/package/nuxt-rollbar-module)
[![npm](https://img.shields.io/npm/dt/nuxt-rollbar-module.svg?style=flat-square)](https://npmjs.com/package/nuxt-rollbar-module)
[![CircleCI](https://img.shields.io/circleci/project/github/Zevran/nuxt-rollbar-module.svg?style=flat-square)](https://circleci.com/gh/Zevran/nuxt-rollbar-module)
[![Codecov](https://img.shields.io/codecov/c/github/Zevran/nuxt-rollbar-module.svg?style=flat-square)](https://codecov.io/gh/Zevran/nuxt-rollbar-module)
[![Dependencies](https://david-dm.org/Zevran/nuxt-rollbar-module/status.svg?style=flat-square)](https://david-dm.org/Zevran/nuxt-rollbar-module)
[![js-standard-style](https://img.shields.io/badge/code_style-standard-brightgreen.svg?style=flat-square)](http://standardjs.com)

> Rollbar module for NuxtJS

## Setup

- Add `nuxt-rollbar-module` dependency using yarn or npm to your project

```shell
npm install --save nuxt-rollbar-module
yarn add nuxt-rollbar-module
```

- Add `nuxt-rollbar-module` to `modules` section of `nuxt.config.js`

```js
{
  modules: [
    // Simple usage
    'nuxt-rollbar-module',

    // With options
    ['nuxt-rollbar-module', {
      serverAccessToken: 'YOUR_ROLLBAR_SERVER_TOKEN',
      clientAccessToken: 'YOUR_ROLLBAR_CLIENT_TOKEN',
      config: {
        // Addtional config
      }
    }],
 ]
}
```

## Usage

Enter your project access tokens in the NuxtJS config file.
See [Rollbar javascript documentation](https://rollbar.com/docs/notifier/rollbar.js/) for options.

### Usage in Vue

```js
Vue.rollbar.debug('Yohyo!');
// or in a vue component
this.rollbar.debug('Yohyo!');
```

## Options

## Development

- Clone this repository
- Install dependencies using `yarn install` or `npm install`
- Start development server using `npm run dev`

## License

[MIT License](./LICENSE)

Copyright (c) Gaël Reyrol <me@gaelreyrol.com>
