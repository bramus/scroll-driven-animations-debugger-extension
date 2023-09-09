# Scroll-Driven Animations Debugger

A DevTools extension to visualize and debug [Scroll-Driven Animations](https://scroll-driven-animations.style/).

- Visualize the Scroll-Driven Animations’s scroller, element, and subject.
- Suppports both ScrollTimeline and ViewTimeline.
- Works with both CSS-based and WAAPI-based Scroll-Driven Animations.
- Plays nice with `position: sticky`.
- Visualize the `animation-range-start` and `animation-range-end`.
- Edit the `animation-range-start` and `animation-range-end` values.

## Demo

https://github.com/bramus/scroll-driven-animations-debugger-extension/assets/213073/4abc106f-9721-4cc9-b909-135b65108f4c

## Installation

You can [get the extension from the Chrome Web Store](https://chromewebstore.google.com/detail/scroll-driven-animations-debugger/ojihehfngalmpghicjgbfdmloiifhoce).

[![Available on the Chrome Web Store](./assets/chrome-webstore.svg)](https://chromewebstore.google.com/detail/scroll-driven-animations-debugger/ojihehfngalmpghicjgbfdmloiifhoce)

If you like this extension, please leave a review on the Chrome Web Store. I’d appreciate it.

## Usage

Once installed, a new “Scroll-Driven Animations” pane gets added to Chrome DevTools’s Elements Panel. To use it, inspect an Element using Chrome DevTools as you’d normally do and select the “Scroll-Driven Animations” pane to see a visualization of the Scroll-Driven Animations that are added to that element. The visualization is a live representation of the scroller, animated element, and – in case of a ViewTimeline – tracked subject: as you scroll in the document, the visualization also updates.

Use the top toolbar to switch between multiple animations _(if more than one)_ or to set the visualization’s scale factor. Typically you don’t need to set the scale factor, as the visualization automatically adapts itself to the available space. Also included in the top toolbar are an indicator telling you which type of scroll timeline you are dealing with, and some progress numbers: total scroll progress, effect progress, actual scroll offset _(in pixels)_.

Use the “Edit Values” toggle at the bottom to bring up a range editor. Once the editor is shown, the visualization also shows indicators for the start and end range. In case of a ScrollTimeline these are two lines on the scroller’s contents. In case of a ViewTimeline these are two boxes representing the areas for the set `animation-range-*` values. Change the values using the dropdown and/or the inputs. Note that the inputs do not live-update _(for now)_; after changing click somewhere outside the field to update the value.

## FAQ

There are some known issues and questions that get asked regularly. Find these in the Issue list with the https://github.com/bramus/scroll-driven-animations-debugger-extension/labels/FAQ label. Note that GitHub by default hides closed issues. To see the full list of FAQ items, use [this direct link](https://github.com/bramus/scroll-driven-animations-debugger-extension/issues?q=label%3AFAQ+)

## Reporting problems / Filing feature requests

Please [file an issue](https://github.com/bramus/scroll-driven-animations-debugger-extension/issues) if you want to report a problem or make a feature request. When reporting a problem, please add a link to a URL where I can reproduce the problem.

## License

This extension is closed source for the time being. This might change over time.