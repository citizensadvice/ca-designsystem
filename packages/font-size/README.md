# Font-size [![npm (scoped)](https://img.shields.io/npm/v/@citizensadvice/font-size.svg)](https://www.npmjs.com/package/@citizensadvice/font-size)

Defines the size of the text.

- [Classes](#classes)
- [Examples](#examples)
- [Installation](#installation)

## Classes

| Class name     | Value                 |
| -------------- | --------------------- |
| `.font-size-1` | `$font-size-1 (14px)` |
| `.font-size-2` | `$font-size-2 (16px)` |
| `.font-size-3` | `$font-size-3 (20px)` |
| `.font-size-4` | `$font-size-4 (28px)` |
| `.font-size-5` | `$font-size-5 (36px)` |

### Responsive font-size classes

To apply specific classes at set screen widths, use the following classes:

| Class name            | Description                                 |
| --------------------- | ------------------------------------------- |
| `[aboveClassName]-ns` | Screens with a min-width of `48rem`         |
| `[aboveClassName]-m`  | Screens with widths from `48rem` to `64rem` |
| `[aboveClassName]-l`  | Screens with a min-width of `64rem`         |

## Examples

```html
<div class="font-size-1 font-size-4-ns">...</div>
<div class="font-size-2 font-size-3-ns font-size-5-l">...</div>
```

## Installation

```shell
$ npm install @citizensadvice/font-size
```

now import into your stylesheet...

```scss
@import '@citizensadvice/font-size/index.scss';
```

You can also make use of the [unpkg](https://unpkg.com) service, try adding the link below to the head of your `HTML` file

```html
<link src="https://unpkg.com/@citizensadvice/font-size@latest/build/font-size.css" />
```
