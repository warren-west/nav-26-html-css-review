# Digitale Talenter 25/26
Revision of HTML and CSS. We've covered:
## HTML
- Open & close tags
- Self-closing tags
- HTML tag names
- HTML attributes
- Block vs inline elements
- Content vs layout elements
- In class I used the [Pexels](https://www.pexels.com) website to find royalty-free images

## CSS
- Using selectors
    1. Tag selectors (least specific)
    2. Class selectors with `.` syntax
    3. ID selectors with `#` syntax (most specific)
- Colors
    - Foreground "text" color with the `color` property
    - Background color with the `background-color` property
    - You can create color `gradients`
        - I showed the [CSS Gradient](https://cssgradient.io/) tool in class
- Borders
    - `border-width`, `border-style`, and `border-color` can be **chained** into a single `border` style.
    - Can be applied to all four sides of a block, or none, or selected sides.
    - `border-radius` to make rounded corners.
- The **box-model** defines how elements on our page take up space
    - Content box
    - Padding can be set using the `padding` CSS property.
    - Border
    - Margins can be set using the `margin` CSS property.
- `padding` and `margin` properties can also use **chaining**, similar to `border`:
    - Values are applied in a clockwise direction, starting from the **top**
    - Or *x* (horizontal) and *y* (vertical) values can be applied, starting with *x*, then *y*.
```css
h1 {
    /* set the margin-top = 12px, margin-right = 10px, margin-bottom = 5px, and margin-left = 0px */
    margin: 12px 10px 5px 0;
    /* set the horizontal padding to 8px, and vertical padding to 4px */
    padding: 8px 4px;
}
```
- Fonts
    - Font sizes can be applied using `px` values, but to keep all fonts sizes on a page relative to one another use `em` or `rem` units of measurement.
        - `em` multiplies the value by the closest parent element that has `font-size` set.
        - `rem` multiples the value by the `:root` element's `font-size` (defaults to 16px).
    - Can use online fonts from CDNs (content delivery networks)
        - We used [Google Fonts](https://fonts.google.com)
    - Icons are also provided by [Google Fonts - Icons](https://fonts.google.com/icons)
- The `filter` property can be used to manipulate an element's:
    - `blur()`
    - `brightness()`
    - `contrast()`
    - `drop-shadow()`
    - `opacity()`
    - `saturate()`
    - and more...
- I applied a `filter` to an `<img>` element's `hover` CSS:
```css
/* When the cursor hovers over the image, make it 10% brighter */
img:hover {
    filter: brightness(110%);
}
```