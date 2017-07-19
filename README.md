# eslint-import-resolver-babel-plugin-root-import

This project fork from [olalonde/eslint-import-resolver-babel-root-import](https://github.com/olalonde/eslint-import-resolver-babel-root-import)

A [babel-plugin-root-import](https://github.com/entwicklerstube/babel-plugin-root-import)
resolver for [eslint-plugin-import](https://github.com/benmosher/eslint-plugin-import).

## Installation

```sh
npm install --save-dev eslint-plugin-import eslint-import-resolver-babel-plugin-root-import
```

## Usage

Inside your `.eslintrc` file, pass this resolver to `eslint-plugin-import`:
```
"settings": {
  "import/resolver": "babel-plugin-root-import"
}
```

And see [babel-plugin-root-import][babel-plugin-root-import] to know how to configure
your prefix/suffix.

### Example

```json
{
  "extends": "airbnb",
  "rules": {},
  "settings": {
    "import/resolver": {
        "babel-plugin-root-import": {
            "rootPathSuffix": "src",
            "rootPathPrefix": "~"
        }
    }
  }
}
```

## License

MIT, see [LICENSE.md](/LICENSE.md) for details.


[babel-plugin-root-import]: https://github.com/entwicklerstube/babel-plugin-root-import
