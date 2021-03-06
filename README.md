*This repository is a mirror of the [component](http://component.io) module [mattcg/stopimmediatepropagation](http://github.com/mattcg/stopimmediatepropagation). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/mattcg-stopimmediatepropagation`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# Polyfill for missing Event#stopImmediatePropagation #

The [stopImmediatePropagation](https://developer.mozilla.org/en-US/docs/DOM/event.stopImmediatePropagation) method can be called on the event object inside a listener to stop other listeners, of the same event type and registered on the same node, being called. Normally, [stopPropagation](https://developer.mozilla.org/en-US/docs/DOM/event.stopPropagation) only stops the event bubbling to parent elements.

The **Android 2** browser has missing support for this wonderful method, so I've extracted this shim from [FastClick](https://github.com/ftlabs/fastclick) and provided a standalone implementation in case anyone needs it.

## License ##

Copyright © 2012 [Matthew Caruana Galizia](http://twitter.com/mcaruanagalizia), licensed under an [MIT license](http://mattcg.mit-license.org/).
