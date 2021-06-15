# Testing NPM local-paths

https://docs.npmjs.com/cli/v7/configuring-npm/package-json#local-paths


## How NPM local-paths works

When adding local path as dependency using `npm install file:./localdep` it creates
symbolic link to local directory.
```bash
  npm install
  ls -alh node_modules
```

>  ... localdep -> ../localdep

Changes to local package are reflected in `node_modules` 🎉.
