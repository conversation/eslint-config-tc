# TC ESLint Configuration

A simple package to keep consistent eslint configuration across our internal apps.

### Usage

1) Install this package
```
npm install --save-dev "https://github.com/conversation/eslint-config-tc"
```

2) Install the correct peer dependencies:
```
npm install --save-dev eslint@^3.15.0 eslint-config-airbnb@^15.1.0 eslint-plugin-import@^2.7.0 eslint-plugin-jsx-a11y@^5.1.1 eslint-plugin-react@^7.1.0
```

3) Add the following to your `.eslintrc.js`
```
module.exports = require('eslint-config-tc')
```

4) Optionally add a convenient way to run eslint and autofix. In `package.json`:
```
"scripts": {
  "lint": "eslint app/assets/javascripts/**/*.jsx",
  "lint:autofix": "eslint --fix app/assets/javascripts/**/*.jsx"
}
```
