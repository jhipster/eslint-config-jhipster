# eslint-config-jhipster-react

Provides [JHipster](https://www.jhipster.tech) [ESLint](https://eslint.org/docs/developer-guide/shareable-configs) shareable configurations used in the JHispter generated React applications.

[![NPM version][npm-image]][npm-url] [![Dependency Status][daviddm-image]][daviddm-url] [![code style: prettier][prettier-image]][prettier-url] [![Downloads][npmcharts-image]][npmcharts-url]

<img src="https://github.com/jhipster/jhipster-artwork/blob/master/logos/JHipster%20RGB-small100x25px.png?raw=true">

## Overview

[JHipster](https://www.jhipster.tech) react shareable configurations.

### Extends

[JHipster](https://www.jhipster.tech) react shareable configuration extends the base set of rules from [eslint-config-jhipster](./base/README.md) to add [react](https://reactjs.org/) specific linting rules.

```
'plugin:react/recommended',
'jhipster'
```

### Rules

In addition to the recommended set of configurations, [JHipster](https://www.jhipster.tech) overrides following rules.

```
    '@typescript-eslint/no-unused-vars': 'off',
    '@typescript-eslint/ban-types': [
      'error',
      {
        types: {
          Object: 'Use {} instead.'
        }
      }
    ],
    '@typescript-eslint/array-type': 'off',
    '@typescript-eslint/unbound-method': 'off',
    'default-case': 'error',
    complexity: ['error', 40],
    'no-invalid-this': 'off',
    'react/prop-types': 'off',
    'react/display-name': 'off'
```

# License

Apache-2.0 © [Vishal Mahajan](https://twitter.com/vishal423)

[npm-image]: https://img.shields.io/npm/v/eslint-config-jhipster-react/latest.svg?style=flat
[npm-url]: https://npmjs.org/package/eslint-config-jhipster-react
[daviddm-image]: https://david-dm.org/jhipster/eslint-config-jhipster-react.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/jhipster/eslint-config-jhipster-react
[prettier-image]: https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square
[prettier-url]: https://github.com/prettier/prettier
[npmcharts-image]: https://img.shields.io/npm/dm/eslint-config-jhipster-react.svg?label=Downloads&style=flat
[npmcharts-url]: https://npmcharts.com/compare/eslint-config-jhipster-react
