# eslint-config-wofh

This package provides WOFH's base JS .eslintrc as an extensible shared config.

## Usage

We export two ESLint configurations for your usage.

### @wofh/eslint-config

Our default export contains all of our ESLint rules, including ECMAScript 6+. It requires `eslint` and `eslint-plugin-import`, `eslint-plugin-react`, `eslint-plugin-react-hooks`.

1. Install the correct versions of each package, which are listed by the command:

  ```sh
  npm info "@wofh/eslint-config@latest" peerDependencies
  ```

  Then run `npm install --save-dev <dependency>@<version>` for each listed peer dependency like the command:

  ```sh
  npm install --save-dev @wofh/eslint-config eslint@^#.#.# eslint-plugin-import@^#.#.# eslint-plugin-react@^#.#.# eslint-plugin-react-hooks@^#.#.#
  ```

2. Add `"extends": "@wofh"` to your .eslintrc.

### @wofh/eslint-config/hooks

This entry point enables the linting rules for React hooks (requires v16.8+). To use, add `"extends": ["@wofh", "@wofh/hooks"]` to your `.eslintrc`

### @wofh/eslint-config/whitespace

This entry point only errors on whitespace rules and sets all other rules to warnings.