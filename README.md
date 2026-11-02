# Newton's Cradle

A Newton's cradle animation built with pure HTML and CSS, no JavaScript. Created as practice with CSS animations, keyframes and transforms.

## Preview

Five white balls hang from a bar on a dark blue background. The outer two swing back and forth in alternation, like the real desk toy.

## How it works

- The cradle is a flex container with five `<span>` elements, one per string.
- Each ball is a `::before` pseudo-element, so the HTML stays minimal.
- `transform-origin: top` makes every string pivot from the bar.
- Only the first and last strings are animated with `@keyframes`. The right one is delayed by 1s, so the two arms swing in turn.

## Usage

Clone or download the repo and open `index.htm` in a browser.

```
cradle/
├── index.htm
└── style.css
```

The Lato font is loaded from Google Fonts, so an internet connection is needed for it to appear.

## Customization

In `style.css` you can tweak:

- `animation` duration and easing on the first and last `span`
- `rotate()` angles in the keyframes to change the swing height
- `height` and `margin` on `.cradle span` to resize the strings and spacing
- `background-color` on `body` to change the background
