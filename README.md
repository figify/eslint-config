# eslint-config

An ESLint [Shareable Config](http://eslint.org/docs/developer-guide/shareable-configs) for web application development using node.js + react

[![gha](https://img.shields.io/github/workflow/status/figify/eslint-config/build)](https://github.com/figify/eslint-config/actions) [![npm](https://img.shields.io/npm/v/@figify/eslint-config)](https://www.npmjs.com/package/@figify/eslint-config) [![license](https://img.shields.io/npm/l/@figify/eslint-config)](./LICENSE)

## Contents

Uses recommended rules from `eslint` the following plugins:

 - import
 - json
 - jsx-a11y
 - eslint-plugin-node
 - eslint-plugin-promise
 - eslint-plugin-react
 - eslint-plugin-security
 - eslint-plugin-sonarjs

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

### React addition

In order not to be bothered by the no unsupported features rule from the node plugin, I add in the folder containing React code another .eslintrc.json file with

```
{
  "rules": {
    "node/no-unsupported-features/es-syntax": "off"
  }
}
```

## Test

    npm test

## License

MIT. Copyright (c) [Kyriakos Chatzidimitriou](http://kyrcha.info).
