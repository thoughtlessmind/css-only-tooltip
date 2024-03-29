# css-only-tooltip

A very lightweight tooltip utility library, made using only `CSS` with dynamic light and dark themes. 

[![NPM downloads](https://badgen.net/npm/dm/css-only-tooltip?icon=npm)](https://www.npmjs.com/package/css-only-tooltip)
[![License](https://badgen.net/npm/license/css-only-tooltip)](https://github.com/thoughtlessmind/css-only-tooltip/blob/main/LICENSE)
![minified size](https://badgen.net/bundlephobia/min/css-only-tooltip?color=pink)
[![npm version](https://img.shields.io/npm/v/css-only-tooltip?color=red)](https://www.npmjs.com/package/css-only-tooltip)
![Css language share](https://img.shields.io/github/languages/top/thoughtlessmind/css-only-tooltip)


![Alt Text](./static/tooltipDemo.gif)

## Installation
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
And then pass the tooltip text in the format:
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
#### When using Package Manager (NPM/Yarn):-
Import the styleSheet into the main  root level component of the App. (for eg. in `App.js` in React App)
```js
import 'css-only-tooltip/dist/styles.min.css';
```
Now, add the text in the `data` attribute in the child components.
```jsx
<span data-css-only-tooltip="Hello from tooltip">Hover on me to see the tooltip</span>
```
## Customization
There are customization options provided.  
Provide the customization options in a space separate string in the data attribute like this:-
``` html
<p data-css-only-props="customization options">
```

### Options:
There are some optional customization options available.
  - #### Positions:
	  There are four positions provided. `Bottom` is the default option.
	  - `top`
	  - `right`
	  - `bottom`
	  - `left`
	 
  - #### Themes:  
	  This supports the user device's theme dynamically. There's no need to specify the theme separately.
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
     Dark tooltip on the right side
  </span>
  ```
_Play with it live:-_  
[![Edit css-only-tooltip-Demo](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/vigilant-nobel-d5qrn?fontsize=14&hidenavigation=1&theme=dark)
