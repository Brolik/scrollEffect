# scrollEffect
Add CSS to an element as it scrolls into view.

## How it works
1. Include the **scrollEffect.js** file anywhere
2. Style the normal state of an element
3. Add the class **scrollEffect** to the element
4. In the stylesheet, write styles for the element when the **queued** class is applied
5. Remember to add a CSS transition to the element for any styles that change
6. On page load, the **queued** class gets added to the element if it's "off screen"
7. When the user scrolls and the element moves into view, the **queued** class is removed

## Example
Fading an image in as it comes into view

```css
img {
    opacity:1;
    transition:opacity .25s ease-out;
}
img.queued {
    opacity:0;
}
```

```html
<img class='scrollEffect' src='...' />
```
