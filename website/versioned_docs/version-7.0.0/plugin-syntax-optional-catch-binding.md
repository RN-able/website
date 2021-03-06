---
id: version-7.0.0-babel-plugin-syntax-optional-catch-binding
title: @babel/plugin-syntax-optional-catch-binding
sidebar_label: syntax-optional-catch-binding
original_id: babel-plugin-syntax-optional-catch-binding
---

## Example

**Syntax**

```javascript
try {
  throw 0;
} catch {
  doSomethingWhichDoesntCareAboutTheValueThrown();
  console.log("Yay, code executes!");
}
```

## Installation

```sh
npm install --save-dev @babel/plugin-syntax-optional-catch-binding
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["@babel/plugin-syntax-optional-catch-binding"]
}
```

### Via CLI

```sh
babel --plugins @babel/plugin-syntax-optional-catch-binding script.js
```

### Via Node API

```javascript
require("@babel/core").transform("code", {
  plugins: ["@babel/plugin-syntax-optional-catch-binding"]
});
```

## References

* [Proposal: Optional Catch Binding for ECMAScript](https://github.com/babel/proposals/issues/7)

