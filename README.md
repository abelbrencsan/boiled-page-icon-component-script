# Boiled Page icon component and script

Icon SCSS component and script for Boiled Page frontend framework. They are intended to use SVG symbols as icons.

## Install

Place `_icon.scss` file to `/assets/css/components` directory, and add its path to components block in `assets/css/app.scss` file.

You will also need to place `icons.js` to `/assets/js` directory and add its path to `scripts` variable in `gulpfile.js` to be combined with other scripts.

## Grid table component

### Classes

Class name | Description | Example
---------- | ----------- | -------
`icon` | Applies an icon with the size of 24x24 pixels. | `<svg class="icon"></svg>`
`icon--16` | Sets icon size to 16x16 pixels. | `<svg class="icon icon--16"></svg>`
`icon--32` | Sets icon size to 32x32 pixels. | `<svg class="icon icon--32"></svg>`
`icon--40` | Sets icon size to 40x40 pixels. | `<svg class="icon icon--40"></svg>`
`icon--64` | Sets icon size to 64x64 pixels. | `<svg class="icon icon--64"></svg>`
`icon--128` | Sets icon size to 64x64 pixels. | `<svg class="icon icon--128"></svg>`
`icon--left` | Applies a narrow margin on the right side of icon. | `<svg class="icon icon--left"></svg>`
`icon--right` | Applies a narrow margin on the right left of icon. | `<svg class="icon icon--left"></svg>`
`icon--baseline` | Sets icon position to the text baseline. | `<svg class="icon icon--baseline"></svg>`

### Examples

#### Example 1

The following example shows an icon.

```html
<svg class="icon" aria-hidden="true">
  <use xlink:href="#icon-arrow-down"></use>
</svg>
```

#### Example 2

The following example shows an icon besides a sample text.

```html
<div>
  Lorem ipsum
  <svg class="icon icon--baseline icon--right" aria-hidden="true">
    <use xlink:href="#icon-arrow-down"></use>
  </svg>
</div>
```

## Icons script

### Usage

```js
// Initialize icons
Icons.init();
```

### Methods

#### Initialize icons

`init()` - Initialize icons. It inserts given symbols into the body.
