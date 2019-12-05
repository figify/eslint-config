# eslint-config

An ESLint [Shareable Config](http://eslint.org/docs/developer-guide/shareable-configs) for web application development using node.js + react

![](https://img.shields.io/github/workflow/status/figify/eslint-config/build)

## Usage

Install as devDependencies the following packages:

    npm install --save-dev @figify/eslint-config eslint-plugin-promise eslint-plugin-import eslint-plugin-node eslint-plugin-json eslint-plugin-jsx-a11y eslint-plugin-react eslint-plugin-security eslint-plugin-sonarjs

or if using *npm 5+* use the shortcut:

    npx install-peerdeps --dev @figify/eslint-config

then create an .eslintrc.json file with

```
{
  extends: "@figify"
}
```

## Test

    npm test

## License

MIT. Copyright (c) [Kyriakos Chatzidimitriou](http://kyrcha.info).
