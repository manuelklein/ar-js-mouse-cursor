# A-Frame Mouse Cursor Component

> **This feature is now available in A-Frame v0.6.1 by setting `<a-scene cursor="rayOrigin: mouse">`.**

This is similar to `cursor` component besides the mouse behaves as cursor.

For detail, please check [cursor page](https://aframe.io/docs/components/cursor.html).

**[DEMO](https://mayognaise.github.io/aframe-mouse-cursor-component/index.html)**

![example](examples/example.gif)

## Properties

There is no property.


## States

The `mouse-cursor` will add states to the cursor entity on certain events.

**There is no `hovering` or `hovered` state for mobile.**

| State Name | Description |
| -------- | ----------- |
| hovering | Added when the cursor is hovering over another entity. |

The cursor will add states to the target entity on certain events.

| State Name | Description |
| -------- | ----------- |
| hovered | Added when target entity is being hovered by the cursor. |


## Events

**There is no `mouseenter` or `mouseleave` events but `click` event for mobile.**

| Event Name | Description |
| -------- | ----------- |
| click | Triggered when an entity is clicked. |
| mouseenter | Triggered on mouseenter of the canvas. |
| mouseleave | Triggered on mouseleave of the canvas. |
| mousedown | Triggered on mousedown of the canvas. |
| mouseup | Triggered on mouseup of the canvas. |

For events, please check [demo page](https://mayognaise.github.io/aframe-mouse-cursor-component/basic/index.html).


## Usage

**The `mouse-cursor` component is usually used alongside the [camera component][components-camera].**

### Browser Installation

Install and use by directly including the [browser files](dist):

```html
<head>
  <title>My A-Frame Scene</title>
  <script src="https://aframe.io/releases/0.5.0/aframe.min.js"></script>
  <script src="https://rawgit.com/mayognaise/aframe-mouse-cursor-component/master/dist/aframe-mouse-cursor-component.min.js"></script>
</head>

<body>
  <a-scene>
    <a-entity camera look-controls mouse-cursor>
  </a-scene>
</body>
```

### NPM Installation

Install via NPM:

```bash
npm i -D aframe-mouse-cursor-component
```

Then register and use.

```js
import 'aframe'
import 'aframe-mouse-cursor-component'
```

### Contributions

If you want to work on this component, take a fork of this branch, and submit a PR back.

* To dev, run `npm run dev` in your terminal, and check your code at `http://localhost:8000`
* To build (prior to PR) run `npm run build`


## Change log

### 0.5.1

- Add ???mousedown??? and ???mouseup??? event

### 0.5.0

- Now works accurately with scenes embedded in page

### 0.2.1

- Now mouse cursor works in stereo mode on both desktop/mobile
- `click` event won't be fired when mouse moves a lot after mouse down


