# Backline Mixins

A scss port of [stylus-mixins](https://github.com/jackbrewer/stylus-mixins), with some added features and modernisation.

TODO:

- [ ] Documentation in progress. For now, read test files for example usage.

## Installation

```sh
npm install --save backline-mixins
```

or

```sh
yarn add backline-mixins
```

Add `backline-mixins` to your node-sass includePaths option.

```js
{
  loader: 'sass-loader',
  options: {
    includePaths: [
      ...require('backline-mixins').includePaths
    ]
  }
}
```

Import backline-mixins in each `.scss` as required

```scss
@import 'backline-mixins';
```

## Changelog

v2.0.0 removes use of / as division operator. Replaces with math.div().

As of v2.0.0 backline-mixins requires dart sass 1.23.0+ to work correctly. SASS:Math (and therefore math:div) is not available in Lib or Ruby SASS, and not on Dart before 1.23.0.

## Development

Clone this repo and install dependencies. All styles have test coverage and Prettier formatting to ensure everything works as expected.

### Running Tests

```sh
yarn test
```

### Updating documentation

This project uses [SassDoc](http://sassdoc.com/) to generate docs using documentation-specific comments.

To regenerate documentation, run:

```sh
yarn docs
```

