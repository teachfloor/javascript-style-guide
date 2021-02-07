# eslint-config-wofh

This package provides WOFH's base JS .eslintrc as an extensible shared config.

## Usage

We export two ESLint configurations for your usage.

### @wofh/eslint-config

Our default export contains all of our ESLint rules, including ECMAScript 6+. It requires `eslint` and `eslint-plugin-import`.

1. Install the correct versions of each package, which are listed by the command:

  ```sh
  npm info "@wofh/eslint-config@latest" peerDependencies
  ```

  Then run `npm install --save-dev <dependency>@<version>` for each listed peer dependency like the command:

  ```sh
  npm install --save-dev @wofh/eslint-config eslint@^#.#.# eslint-plugin-import@^#.#.#
  ```

2. Add `"extends": "wofh"` to your .eslintrc.
