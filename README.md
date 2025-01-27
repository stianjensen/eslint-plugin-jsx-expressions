# eslint-plugin-jsx-expressions

Rules for safe logical expressions in JSX

## Installation

You'll first need to install [ESLint](https://eslint.org/):

```sh
npm i eslint --save-dev
```

Next, install `@jgoz/eslint-plugin-jsx-expressions`:

```sh
npm install @jgoz/eslint-plugin-jsx-expressions --save-dev
```

## Usage

Add `@jgoz/jsx-expressions` to the plugins section of your `.eslintrc` configuration file. You can omit the `eslint-plugin-` prefix:

```json
{
  "plugins": ["@jgoz/jsx-expressions"]
}
```

Then configure the rules you want to use under the rules section.

```json
{
  "rules": {
    "@jgoz/jsx-expressions/strict-logical-expressions": "error"
  }
}
```

## Supported Rules

- [jsx-expressions/strict-logical-expressions](https://github.com/jgoz/eslint-plugin-jsx-expressions/blob/master/docs/rules/strict-logical-expressions.md): Enforces logical "&&" expressions do not use potentially falsey numbers or strings.
