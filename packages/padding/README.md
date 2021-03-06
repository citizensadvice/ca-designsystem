# Padding [![npm (scoped)](https://img.shields.io/npm/v/@citizensadvice/padding.svg)](https://www.npmjs.com/package/@citizensadvice/padding)

Defines the space inside an element.

- [Abbreviations](#abbreviations)
- [Examples](#examples)
- [Installation](#installation)

## Abbreviations

| Abbr | Value                        |
| ---- | ---------------------------- |
| `p`  | padding                      |
| `t`  | top                          |
| `r`  | right                        |
| `pb` | bottom                       |
| `pl` | left                         |
| `pv` | vertical, top & bottom       |
| `ph` | horizontal, left & right     |
| `0`  | `$spacing-0` (0rem, 0px)     |
| `1`  | `$spacing-1` (0.25rem, 4px)  |
| `2`  | `$spacing-2` (0.5rem, 8px)   |
| `3`  | `$spacing-3` (0.75rem, 12px) |
| `4`  | `$spacing-4` (1rem, 16px)    |
| `5`  | `$spacing-5` (1.5rem, 24px)  |
| `6`  | `$spacing-6` (2rem, 32px)    |
| `7`  | `$spacing-7` (2.5rem, 40px)  |

## Examples

### Uniform padding

```html
<div class="p-0">Lorem ipsum</div>
<div class="p-1">Lorem ipsum</div>
<div class="p-2">Lorem ipsum</div>
<div class="p-3">Lorem ipsum</div>
<div class="p-4">Lorem ipsum</div>
<div class="p-5">Lorem ipsum</div>
<div class="p-6">Lorem ipsum</div>
<div class="p-7">Lorem ipsum</div>

// This will give a padding of x to all sides.
```

### Directional padding

```html
<div class="pt-4">Lorem ipsum</div>
// This will give a padding-top of 16px.

<div class="pr-3">Lorem ipsum</div>
// This will give a padding-right of 12px.

<div class="pb-5">Lorem ipsum</div>
// This will give a padding-bottom of 24px.

<div class="pl-7">Lorem ipsum</div>
// This will give a padding-left of 40px.
```

### Responsive padding classes

To apply specific classes at set screen widths, use the following classes:

| Abbr | Value                                                |
| ---- | ---------------------------------------------------- |
| `ns` | `$breakpoint-ns` (min-width: 48rem)                  |
| `m`  | `$breakpoint-m` (min-width: 48rem, max-width: 64rem) |
| `l`  | `$breakpoint-l` (min-width: 64rem)                   |

```html
<div class="pl-7-l pl-5-ns pl-3">Lorem ipsum</div>

// This will give a padding-left of 40px on device widths over 64rem, 24px on devices with a width
of 48rem and finally 12px on devices with a width up to 48rem.
```

## Installation

```shell
$ npm install @citizensadvice/padding
```

now import into your stylesheet...

```scss
@import '@citizensadvice/padding/index.scss';
```

You can make use of the [unpkg](https://unpkg.com) service, try adding the link below to the head of your `HTML` file.

```html
<link src="https://unpkg.com/@citizensadvice/padding@latest/build/padding.css" />
```
