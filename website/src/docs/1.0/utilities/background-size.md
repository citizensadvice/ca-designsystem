---
layout: docs
title: Colours
---
# Background-size

| Name                              | Type   | Version                                                                           |
|-----------------------------------|--------|-----------------------------------------------------------------------------------|
| `@citizensadvice/background-size` | Utilty | ![npm (scoped)](https://img.shields.io/npm/v/@citizensadvice/background-size.svg) |

## Dependencies

| Name                      | Description                 |
|---------------------------|-----------------------------|
| `@citizensadvice/support` | System wide settings/config |

## Installation

Using your package manager of choice...

```shell
$ npm install @citizensadvice/background-size
```

Then bring into your stylesheets with...

```scss
@import "@citizensadvice/background-size/index.scss";
```

### OR
You can also make use of the [unpkg](https://unpkg.com) service, try adding the link below to the head of your `HTML` file

```html
<link src="https://unpkg.com/@citizensadvice/background-size@latest/build/background-size.css"/>
```

## Introduction

Defines the size of the background image.

```CSS
.bg-cover   { background-size: cover   }
.bg-contain { background-size: contain }
```

## Responsive background-size classes

To apply specific classes at set screen widths, use the following classes:

| Available classes     | Description                                 |
|-----------------------|---------------------------------------------|
| `[aboveClassName]-ns` | Screens with a min-width of `48rem`         |
| `[aboveClassName]-m`  | Screens with widths from `48rem` to `64rem` |
| `[aboveClassName]-l`  | Screens with a min-width of `64rem`         |

### Example markup

```html
<div class="bg-contain bg-cover-ns">...</div>
```
