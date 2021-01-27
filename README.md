# css-only-tooltip

A very lightweight tooltip utitlity library, made using only `CSS` with dynamic light and dark themes. 

[![Node.js Package](https://github.com/thoughtlessmind/css-only-tooltip/workflows/Node.js%20Package/badge.svg)](https://github.com/thoughtlessmind/css-only-tooltip)
[![NPM downloads](https://badgen.net/npm/dm/css-only-tooltip?icon=npm)](https://www.npmjs.com/package/css-only-tooltip)
[![License](https://badgen.net/npm/license/css-only-tooltip)](https://github.com/thoughtlessmind/css-only-tooltip/blob/main/LICENSE)
![minified size](https://badgen.net/bundlephobia/min/css-only-tooltip?color=pink)
[![npm version](https://badgen.net/npm/v/css-only-tooltip)](https://www.npmjs.com/package/css-only-tooltip)
![npm version](https://img.shields.io/github/languages/top/thoughtlessmind/css-only-tooltip)


## Insatallation
- Using npm  
		`$ npm install css-only-tooltip`  
		
- Using yarn  
		`$ yarn add css-only-tooltip`

- Using jsDelivr CDN
	```html
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/css-only-tooltip@latest/dist/styles.min.css">
	```


- Using unpkg CDN:
	```html
	<link rel="stylesheet" href="https://unpkg.com/css-only-tooltip@latest/dist/styles.min.css">
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
#### When using Package Manger (NPM/Yarn):-
Import the styleSheet into the main  root level component of the App. (for eg. in `App.js` in React App)
```js
import 'css-only-tooltip/dist/styles.min.css';
```
Now, add the text in the `data` attribute in the child components.
```jsx
<data-css-only-tooltip="Hello from tooltip">Hover on me to see the tooltip</span>
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
	  This supports the user device's theme dynamically. There's no need to specify theme spereately.
	  Beside this, there are two theme options provided for customization. `light` is default option.
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
