# prettier-config-webchannel

> Sharing a Prettier configuration [Prettier](https://prettier.io) config.


<img src="https://www.wisdomgeek.com/wp-content/uploads/2018/02/prettier.png"
alt="Showreel" width="100%" border="10" />

## Installation

```sh
yarn add --dev prettier-config-webchannel
```
or

```sh
npm install prettier-config-webchannel --save-dev
```

## Usage
In your `package.json`:
```javascript
{
  "name": "my-library",
  "version": "1.0.0",
  "prettier": "prettier-config-webchannel"
}
```

If you don't want to use your `package.json`, you can create a `.prettierrc.json` file in your projects root directory.
```javascript
"prettier-config-webchannel"
```

If you would like to extend or modify these properties, create a `.prettierrc.js` file in your projects root directory and export your desired modifications.
```javascript
module.exports = {
  ...require('prettier-config-webchannel'),
  printWidth: 120
};
```

## Properties

### <a href="https://github.com/airbnb/javascript/blob/master/README.md#objects--quoted-props">3.6</a> Quote Props
> Only quote properties that are invalid identifiers.

`"quoteProps": "as-needed"`

### <a href="https://github.com/airbnb/javascript/blob/master/README.md#strings--quotes">6.1</a> Quotes
> Use single quotes instead of double quotes.

`"singleQuote": true`

### <a href="https://github.com/airbnb/javascript/blob/master/README.md#arrows--implicit-return">8.2</a> Arrow Function Parentheses
> Remove parentheses around a sole arrow function parameter.

`"arrowParens": "avoid"`

### <a href="https://github.com/airbnb/javascript/blob/master/README.md#whitespace--max-len">19.1</a> Tabs and Tab Width
> Use soft tabs (space character) set to 2 spaces.

`"tabWidth": 2`

`"useTabs": false`

### <a href="https://github.com/airbnb/javascript/blob/master/README.md#whitespace--max-len">19.3</a> Print Width and Wrapping
> Specify the line length that the printer will wrap on. Wrap prose if it exceeds the print width.

`"printWidth": 100`

`"proseWrap": "preserve"`

### <a href="https://github.com/airbnb/javascript/blob/master/README.md#whitespace--in-brackets">19.11</a> Bracket Spacing
> Do not print spaces between brackets in object literals.

`"bracketSpacing": false`

### <a href="https://github.com/airbnb/javascript/blob/master/README.md#commas--dangling">20.2</a> Trailing Commas
> Print trailing commas wherever possible when multi-line. (A single-line array, for example, never gets trailing commas.)

`"trailingComma": "es5"`

### <a href="https://github.com/airbnb/javascript/blob/master/README.md#semicolons--required">21.1</a> Semicolons
> Print semicolons at the ends of statements.

`"semi": true`

## JSX Properties
Prettier allows some React/JSX properties to be configured. If your project doesn't use React, no need to worry; these properties won't be applied to your project!

### <a href="https://github.com/airbnb/javascript/blob/master/README.md#objects--quoted-props">Quotes</a>
> Use double quotes in JSX.

`"jsxSingleQuote": false`

### <a href="https://github.com/airbnb/javascript/tree/master/react#tags">Tags</a>
> If your component has multi-line properties, close its tag on a new line.

`"jsxBracketSameLine": false`
