# craco-linaria3

craco-linaria is not support linaria3, So update some file.

A [craco](https://www.npmjs.com/package/@craco/craco) plugin to use [Linaria][]
zero-runtime CSS in JS library in a create react app.

## Installation

First, follow craco's
[installation instructions](https://github.com/sharegate/craco/blob/master/packages/craco/README.md#installation).

Then, install `craco-linaria3` and [Linaria][]:

```bash
$ yarn add  @linaria/core @linaria/react
and
$ yarn add craco-linaria3 @linaria/babel @linaria/webpack4-loader -D
```

## Usage

```js
/* craco.config.js */
const CracoLinariaPlugin = require('craco-linaria3')

module.exports = {
  plugins: [
    {
      plugin: CracoLinariaPlugin,
      options: {
        // Linaria options
      },
    },
  ],
}
```

You can specify
[Linaria options](https://github.com/callstack/linaria/blob/master/docs/CONFIGURATION.md#options)
inline (as above) or it will be picked up from any of the
[supported configuration paths](https://github.com/callstack/linaria/blob/master/docs/CONFIGURATION.md#configuration).

## Git Ignore

This plugin stores [Linaria][] cache in `src/.linaria_cache`, so you might want
to add that path to your [`.gitignore`](https://git-scm.com/docs/gitignore)
file.

[linaria]: https://linaria.now.sh/

## Thanks

[craco-linaria](https://github.com/jedmao/craco-linaria.git)
