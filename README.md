# TC ESLint Configuration

A simple package to keep consistent eslint configuration across our internal apps.

### Usage

1) Install this package
```
npm install --save-dev eslint-config-tc
```

2) Install the correct peer dependencies, which you can find by using the command
```
npm info "https://github.com/conversation/eslint-config-tc@latest" peerDependencies
```

3) Add the following to your `.eslintrc.js`
```
module.exports = require('eslint-config-tc')
```

4) Optionally add a convenient way to run eslint and autofix. In `package.json`:
```
...
"scripts": {
  "lint": "eslint app/assets/javascripts/**/*.jsx",
  "lint:autofix": "eslint --fix app/assets/javascripts/**/*.jsx"
},
...
```
