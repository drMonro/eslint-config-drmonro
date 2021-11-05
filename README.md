# eslint-config-drmonro

ESLint [shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html)

## Installation

```bash
npm install --save-dev eslint-config-drmonro
```

Package requires `eslint`. You must install it manually.

## Usage

Once the `eslint-config-drmonro` package is installed, you can use it by specifying `drmonro` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

For validating **Vanilla JS** project use `vanilla` version:

```json
{
  "parserOptions": {
    "ecmaVersion": 2018,
    "sourceType": "module"
  },
  "env": {
    "es2017": true,
    "browser": true
  },
  "extends": "htmlacademy/vanilla",
  "rules": {
    // Additional rules...
  }
}
```

For validating **React** project use `react` version (`htmlacademy/react` includes `react/recommended`):

```json
{
  "parserOptions": {
    "ecmaVersion": 2018,
    "sourceType": "module"
  },
  "env": {
    "es2017": true,
    "browser": true
  },
  "extends": "drmonro/react",
  "rules": {
    // Additional rules...
  }
}
```

For validating **React** project with TypeScript use `react-typescript` version (`drmonro/react-typescript` includes `react/recommended` and `@typescript-eslint/recommended`):

```json
{
  "parserOptions": {
    "ecmaVersion": 2018,
    "sourceType": "module"
  },
  "env": {
    "es2017": true,
    "browser": true
  },
  "extends": "drmonro/react-typescript",
  "rules": {
    // Additional rules...
  }
}
```

Caution! `drmonro/react` and `drmonro/react-typescript` doesn't include `react-hooks/rules-of-hooks` and `react-hooks/exhaustive-deps` because i use CRA (Create React App) which includes these plugins out of box. Install them yourself if necessary.

**Node.js** versions soon.
