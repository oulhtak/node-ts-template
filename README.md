### NodeJS start up template that supports:

- ESLint ([`.eslintrc.js`](./.eslintrc.js))
- Prettier ([`.prettierrc`](./.prettierrc))
- Typescript ([`tsconfig.json`](./tsconfig.json))
- `eslint-config-prettier` (helps eslint and prettier get along)

### Auto-formatting on save:

Inside `/.vscode/settings.json` we set prettier as the default formatter, and also set `editor.codeActionsOnSave` to run:

- **Lint:** `"source.fixAll.eslint"`
- **Format:** `"source.fixAll.format"`

### Checking standards pre-commit:

Using [husky](https://www.npmjs.com/package/husky) we can check all of our style standards to make sure our git commits are up to par. Check those checks out at [`.husky/pre-commit`](.husky/pre-commit)

### build

yarn build will create a dist folder that inludes that js files

It's advisable to use yarn over npm
