# eslint-config-jhipster

Provides [JHipster](https://www.jhipster.tech) [ESLint](https://eslint.org/docs/developer-guide/shareable-configs) shareable configurations used in the JHispter frontend Typescript/Javascript applications.

[![NPM version][npm-image]][npm-url] [![Dependency Status][daviddm-image]][daviddm-url] [![code style: prettier][prettier-image]][prettier-url] [![Downloads][npmcharts-image]][npmcharts-url]

<img src="https://github.com/jhipster/jhipster-artwork/blob/master/logos/JHipster%20RGB-small100x25px.png?raw=true">

## Overview

It contains frontend framework-agnostic base set of eslint rules. These rules help us to deliver consistent code quality across different frontend framework implementations supported by [JHipster](https://www.jhipster.tech).

### Extends

To keep consistent code quality across different implementations, [JHipster](https://www.jhipster.tech) shareable configuration extends the following set of recommended `ESLint` and `Typescript` configurations. JHipster uses `prettier` to keep consistent code formatting.

```
'eslint:recommended',
'plugin:@typescript-eslint/eslint-recommended',
'plugin:@typescript-eslint/recommended',
'plugin:@typescript-eslint/recommended-requiring-type-checking',
'prettier',
'prettier/@typescript-eslint',
'eslint-config-prettier'
```

### Rules

In addition to the recommended set of configurations, [JHipster](https://www.jhipster.tech) overrides following rules.

```
'@typescript-eslint/member-ordering': [
      'error',
      {
        default: [
          'static-field',
          'instance-field',
          'constructor',
          'static-method',
          'instance-method'
        ]
      }
    ],
    '@typescript-eslint/no-parameter-properties': [
      'warn',
      { allows: ['public', 'private', 'protected'] }
    ],
    '@typescript-eslint/no-unused-vars': [
      'warn',
      {
        vars: 'all',
        args: 'none',
        ignoreRestSiblings: false
      }
    ],
    '@typescript-eslint/explicit-member-accessibility': 'off',
    '@typescript-eslint/explicit-function-return-type': 'off',
    '@typescript-eslint/no-explicit-any': 'off',
    '@typescript-eslint/ban-types': 'off',
    '@typescript-eslint/interface-name-prefix': 'off',
    '@typescript-eslint/no-empty-function': 'off',
    '@typescript-eslint/unbound-method': 'off',
    'spaced-comment': ['warn', 'always'],
    'guard-for-in': 'error',
    'no-labels': 'error',
    'no-caller': 'error',
    'no-bitwise': 'error',
    'no-console': ['error', { allow: ['warn', 'error'] }],
    'no-new-wrappers': 'error',
    'no-eval': 'error',
    'no-shadow': 'error',
    'no-new': 'error',
    'no-var': 'error',
    radix: 'error',
    eqeqeq: ['error', 'always', { null: 'ignore' }],
    'prefer-const': 'error',
    'object-shorthand': ['error', 'always', { avoidExplicitReturnArrows: true }]
```

# License

Apache-2.0 © [Vishal Mahajan](https://twitter.com/vishal423)

[npm-image]: https://img.shields.io/npm/v/eslint-config-jhipster/latest.svg?style=flat
[npm-url]: https://npmjs.org/package/eslint-config-jhipster
[daviddm-image]: https://david-dm.org/jhipster/eslint-config-jhipster.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/jhipster/eslint-config-jhipster
[prettier-image]: https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square
[prettier-url]: https://github.com/prettier/prettier
[npmcharts-image]: https://img.shields.io/npm/dm/eslint-config-jhipster.svg?label=Downloads&style=flat
[npmcharts-url]: https://npmcharts.com/compare/eslint-config-jhipster
