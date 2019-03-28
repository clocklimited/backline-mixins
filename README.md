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

## Development

Clone this repo and install dependencies. All styles have test coverage and Prettier formatting to ensure everything works as expected.

### Running Tests

```sh
yarn test
```

### Updateing docs

This project uses [SassDoc](http://sassdoc.com/) to generate documentation using documentation-specific comments.

To regenerate documentation, run:

```sh
yarn docs
```

