---
id: babel-plugin-transform-sticky-regex
title: @babel/plugin-transform-sticky-regex
sidebar_label: transform-sticky-regex
---

## Examples

**In**

```javascript
const a = /o+/y;
```

**Out**

```javascript
var a = new RegExp("o+", "y");
```

## Installation

```sh
npm install --save-dev @babel/plugin-transform-sticky-regex
```

## Usage

### With a configuration file (Recommended)

```json
{
  "plugins": ["@babel/plugin-transform-sticky-regex"]
}
```

### Via CLI

```sh
babel --plugins @babel/plugin-transform-sticky-regex script.js
```

### Via Node API

```javascript
require("@babel/core").transform("code", {
  plugins: ["@babel/plugin-transform-sticky-regex"]
});
```

