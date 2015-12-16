# react-native-parallax-scroll-view

A `ScrollView`-like component with parallax and sticky header support.

Tested with react-native 0.16.0 on Android and iOS.

## Installation

```
$ npm install react-native-parallax-scroll-view --save
```

## Demo

![](./parallax-scroll-view-ios.gif)

## Example

Please refer to the [Example](./Example/example.js) provided.

## Usage (API)

All of the properties of `ParallaxScrollView` are supported. Please refer to the
[`ParallaxScrollView` documentation](https://facebook.github.io/react-native/docs/scrollview.html) for more detail.

The `ParallaxScrollView` component adds a few additional properties, as described below.

| Property | Type | Required | Default | Description |
| -------- | ---- | -------- | ------- | ----------- |
| `renderParallaxHeader` |  `func` | Yes | N/A | This renders the parallax header above the background. |
| `parallaxHeaderHeight` | `number` | Yes | This is the initial height of parallax header. |
| `backgroundColor` | `string` | No | `'#000'` | This is the background color of sticky header, and also used as parallax header background color if `renderBackground` is not provided. |
| `renderBackground` | `func` | No | Opaque background using `backgroundColor`. | This renders the background of the parallax header. Can be used to display cover images for example. |
| `renderStickyHeader` | `func` | No | N/A | This renders an optional sticky header that will stick to the top of view when parallax header scrolls up. |
| `stickyHeaderHeight` | `number` | If `renderStickyHeader` is used | 0 | If `renderStickyHeader` is set, then its height must be specified. |
| `renderFixedHeader` | `func` | No | N/A | This renders an optional fixed header that will always be visible and fixed to the top of the view (and sticky header). You must set its height and width appropriately. |
