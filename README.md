# css-only-tooltip

[![Node.js Package](https://github.com/thoughtlessmind/css-only-tooltip/workflows/Node.js%20Package/badge.svg)](https://github.com/thoughtlessmind/css-only-tooltip)
[![NPM downloads](https://badgen.net/npm/dm/css-only-tooltip?icon=npm)](https://www.npmjs.com/package/css-only-tooltip)
[![License](https://badgen.net/npm/license/css-only-tooltip)](https://github.com/thoughtlessmind/css-only-tooltip/blob/main/LICENSE)
![minified size](https://badgen.net/bundlephobia/min/css-only-tooltip?color=pink)
[![npm version](https://badgen.net/npm/v/css-only-tooltip)](https://www.npmjs.com/package/css-only-tooltip)
![npm version](https://img.shields.io/github/languages/top/thoughtlessmind/css-only-tooltip)

A very lightweight tooltip utitlity library, made using only `CSS`. 

## Insatallation
- Using npm
		`$ npm install css-only-tooltip`  
		
- Using yarn
		`$ yarn add css-only-tooltip`

- Using jsDelivr CDN
	```js
	<script src="https://cdn.jsdelivr.net/npm/css-only-tooltip@latest/dist/styles.min.css"></script>
	```


- Using unpkg CDN:
	```js
	<script src="https://unpkg.com/css-only-tooltip@latest/dist/styles.min.css"></script>
	```

## Quick start
`css-only-tooltip` uses only `data` html attribute for working. So, the only step is to import the `CSS`  in your file and use it.

#### When using CDN:-
Add the CDN link in your `HTML` file inside the `<head>` tag. 
And then pass the tooltip text in format:
 ```html
 <!DOCTYPE  html>
  <head>
    <!-- Add the CDN link -->
    <link rel="stylesheet" href="https://unpkg.com/css-only-tooltip@0.0.12/dist/styles.min.css">
</head>

<body>
    <div class="container">
      <p data-css-only-tooltip="Tooltip 1">Text</p>
    </div>
</body>
</html>
 ```

## Customization
There are customization options provided.  
Provide the customization options in a space seperated string in the data attribute like this:-
``` html
<p data-css-only-props="customization options">
```

### Options:
Thre are some optional customization options are available.
  - #### Positions:
	  There are four positions provided. `Bottom` is default option.
	  - `top`
	  - `right`
	  - `bottom`
	  - `left`
	 
  - #### Themes:
	  There are two theme options provided. `light` is default option.
	  - `dark`
	  - `light`
---
|Option| Values | default | Required |
|--|--|--|--|
| Position | `top`, `right`, `bottom`, `left` | `bottom` | No |
|Theme|`light`, `dark`|`light`|No|
--- 


### Examples:
- dark theme, right side.
  ```html
  <span 
    data-css-only-tooltip="Tooltip 2 bottom" 
    data-css-only-tooltip-props="light bottom">
     Dakr tooltip on right side
  </span>
  ```
