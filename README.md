# React DnD HTML5 Backend [![npm package](https://img.shields.io/npm/v/react-dnd-html5-backend.svg?style=flat-square)](https://www.npmjs.org/package/react-dnd-html5-backend)

This is a modified version for compatibility with FineUploader.  FineUploader stops the drop event from propogating which causes the html5 backend to get stuck in a dragging state.  This version makes sure to end all native drag events.


The officially supported HTML5 backend for [React DnD](http://gaearon.github.io/react-dnd/).
See [the docs](http://gaearon.github.io/react-dnd/docs-html5-backend.html) for usage information.

## Installation

If you use [npm](http://npmjs.com):

```
npm install --save react-dnd-html5-backend
```

The npm package defaults to the CommonJS build.

However it also includes a pre-minified UMD build in the `dist` folder.
The UMD build exports a global `window.ReactDnDHTML5Backend` when imported as a `<script>` tag.

If you’d rather not use npm, you can use [npmcdn](http://npmcdn.com/) to access the UMD build directly: [ReactDnDHTML5Backend.min.js](https://npmcdn.com/react-dnd-html5-backend@latest/dist/ReactDnDHTML5Backend.min.js).
You may point your Bower config to it.

## Browser Support

We strive to support the evergreen browsers, Safari 7+, as well as IE11+. IE10 should also work, but `DragLayer` is fairly useless because IE10 doesn’t support `pointer-events: none`. We don’t officialy support IE9 and less.

Unfortunately the browser bugs, inconsistencies, and regressions come up from time to time, so please make sure you test your app on the browsers you’re interested in, and report any bugs to us.

## License

MIT
