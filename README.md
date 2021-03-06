# Toasteo JS
A simple Toast package that is lightweight (5kb~) with zero dependencies written in vanilla JS

## Getting started
#### [Install from npm](https://www.npmjs.com/package/toasteo)
```
npm install --save-dev toasteo
```

#### In your JS file
```
import Toasteo from "toasteo";
window.Toasteo = new Toasteo({});
```

## Basic usage
There is four toasts ready to be used, a success toast, an error toast, a warning toast and an info toast. They all use the same syntax, the only difference is the style applied.

```
window.Toasteo.success('My success toast');
window.Toasteo.error('My error toast');
window.Toasteo.warning('My warning toast');
window.Toasteo.info('My info toast');
```

This all works by default using the provided CSS.

## Options
You can change the default options when initializing the package.
```
window.Toasteo = new Toasteo(options};
```

| Option | Description | Default |
|:-------------:|:-------------|:-----:|
| prependTo     | The dom element that the toast notification will be prepended to. | `document.body.childNodes[0]` |
|  duration  | The duration after which the toast will be removed.      |   `4000` (ms) |
| animateOnRemoving | Animate the toast when removing it by adding a CSS class. | `true` |
| animationRemovingDuration | The duration of the remove animation in milliseconds, after which the toast will be removed from the DOM | `400` |
| animateOnCreation | Animate the toast when creating it by adding a CSS class. | `true` |
| closeOnClick | The toast should be removed when clicked. | `true` |
| classes | The default classes used by the package. | `{container: 'toast-container', default: 'toast', closing: 'toast--closing', creating: 'toast--creating', 'success': 'toast--success', 'error': 'toast--error', 'warning': 'toast--warning', 'info': 'toast--info'}` |

## Demo & Documentation
You can see Toasteo in action on the [demo page](https://fhusquinet.github.io/toasteo-js/) as well as a better documentation.