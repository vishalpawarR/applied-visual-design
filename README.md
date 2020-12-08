# applied-visual-design

CSS visual design topics

## 1-text-align :

- `text-align: justify;` causes all lines of text except the last line to meet the left and right edges of the line box.
- `text-align: center;` centers the text

- `text-align: right;` right-aligns the text

- `text-align: left;` (the default) left-aligns the text.

## 2 - width :

```css
img {
  width: 220px;
}
```

- You can specify the width of an element using the width property in CSS. Values can be given in relative length units (such as em), absolute length units (such as px), or as a percentage of its containing parent element. Here's an example that changes the width of an image to 220px:

## 3 - height :

```css
img {
  height: 20px;
}
```

- You can specify the height of an element using the height property in CSS, similar to the width property. Here's an example that changes the height of an image to 20px:

## 4 - font-weight: bold :

- To make text bold, you can use the strong tag. This is often used to draw attention to text and symbolize that it is important. With the strong tag, the browser applies the CSS of font-weight: bold; to the element.

## 5 - font-decoration:underline :

- To underline text, you can use the u tag. This is often used to signify that a section of text is important, or something to remember. With the u tag, the browser applies the CSS of text-decoration: underline; to the element.

## 6 - font-style italic :

- To emphasize text, you can use the em tag. This displays text as italicized, as the browser applies the CSS of font-style: italic; to the element.

## 7 - text-decoration: line-through :

- To strikethrough text, which is when a horizontal line cuts across the characters, you can use the s tag. It shows that a section of text is no longer valid. With the s tag, the browser applies the CSS of text-decoration: line-through; to the element.

## 8 - hr :

- You can use the hr tag to add a horizontal line across the width of its containing element. This can be used to define a change in topic or to visually separate groups of content.

## 9 - background-color: rgba() :

- Instead of adjusting your overall background or the color of the text to make the foreground easily readable, you can add a background-color to the element holding the text you want to emphasize. This challenge uses rgba() instead of hex codes or normal rgb().

```
rgba stands for:
  r = red
  g = green
  b = blue
  a = alpha/level of opacity
```

- The RGB values can range from 0 to 255. The alpha value can range from 1, which is fully opaque or a solid color, to 0, which is fully transparent or clear. rgba() is great to use in this case, as it allows you to adjust the opacity. This means you don't have to completely block out the background.

- You'll use background-color: rgba(45, 45, 45, 0.1) for this challenge. It produces a dark gray color that is nearly transparent given the low opacity value of 0.1.

## 10 - font-size:

- The font size of header tags (h1 through h6) should generally be larger than the font size of paragraph tags. This makes it easier for the user to visually understand the layout and level of importance of everything on the page. You use the font-size property to adjust the size of the text in an element.

## 11 - box-shadow :

- The `box-shadow` property applies one or more shadows to an element.

- The `box-shadow property` takes values for

  - `offset-x` (how far to push the shadow horizontally from the element),
  - `offset-y` (how far to push the shadow vertically from the element),
  - `blur-radius`,
  - `spread-radius` and
  - `color`, in that order.
    The `blur-radius` and `spread-radius` values are optional.

- Multiple box-shadows can be created by using commas to separate properties of each `box-shadow` element.

* Here's an example of the CSS to create multiple shadows with some blur, at mostly-transparent black colors:

```css
box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
```

### 12 - Opacity :

- The `opacity` property in CSS is used to adjust the opacity, or conversely, the transparency for an item.

```css
A value of 1 is opaque, which isn't transparent at all.
A value of 0.5 is half see-through.
A value of 0 is completely transparent.
```

- The value given will apply to the entire element, whether that's an image with some transparency, or the foreground and background colors for a block of text.

## 13 - text-transform :

- The text-transform property in CSS is used to change the appearance of text. It's a convenient way to make sure text on a webpage appears consistently, without having to change the text content of the actual HTML elements.

* The following table shows how the different text-transformvalues change the example text "Transform me".

| Value      | Result                                               |
| ---------- | ---------------------------------------------------- |
| lowercase  | "transform me"                                       |
| uppercase  | "TRANSFORM ME"                                       |
| capitalize | "Transform Me"                                       |
| initial    | Use the default value                                |
| inherit    | Use the text-transform value from the parent element |
| none       | Default: Use the original text                       |

## 14 - font-size :

- The font-size property is used to specify how large the text is in a given element. This rule can be used for multiple elements to create visual consistency of text on a page. In this challenge, you'll set the values for all h1 through h6 tags to balance the heading sizes.

## 15 - font-weight :

- You set the font-size of each heading tag in the last challenge, here you'll adjust the font-weight.

- The font-weight property sets how thick or thin characters are in a section of text.

## 16 - font-size :

- The font-size property in CSS is not limited to headings, it can be applied to any element containing text.

## 17 - line-height :

- CSS offers the line-height property to change the height of each line in a block of text. As the name suggests, it changes the amount of vertical space that each line of text gets.

# pseudo-classes :

## 18 - :hover :

- This challenge will touch on the usage of pseudo-classes. A pseudo-class is a keyword that can be added to selectors, in order to select a specific state of the element.

- For example, the styling of an anchor tag can be changed for its hover state using the `:hover` pseudo-class selector. Here's the CSS to change the `color` of the anchor tag to red during its hover state:

```css
<style>
  a {
    color: #000;
  }
  a:hover {
    color: blue;
  }
</style>
```

## 19 - Relative position :

- CSS treats each HTML element as its own box, which is usually referred to as the **CSS Box Model**. Block-level items automatically start on a new line (think headings, paragraphs, and divs) while inline items sit within surrounding content (like images or spans). The default layout of elements in this way is called the normal flow of a document, but CSS offers the position property to override it.

- When the position of an element is set to `relative`, it allows you to specify how CSS should move it relative to its current position in the normal flow of the page. It pairs with the CSS offset properties of `left` or `right`, and `top` or `bottom`. These say how many pixels, percentages, or ems to move the item away from where it is normally positioned. The following example moves the paragraph 10 pixels away from the bottom:

```css
p {
  position: relative;
  bottom: 10px;
}
```

- Changing an element's position to relative does not remove it from the normal flow - other elements around it still behave as if that item were in its default position. **Note:** Positioning gives you a lot of flexibility and power over the visual layout of a page. It's good to remember that no matter the position of elements, the underlying HTML markup should be organized and make sense when read from top to bottom. This is how users with visual impairments (who rely on assistive devices like screen readers) access your content.

## 20 - relative-offset :

- The CSS offsets of top or bottom, and left or right tell the browser how far to offset an item relative to where it would sit in the normal flow of the document. You're offsetting an element away from a given spot, which moves the element away from the referenced side (effectively, the opposite direction). As you saw in the last challenge, using the top offset moved the h2 downwards. Likewise, using a left offset moves an item to the right.
  ![this is offset](https://cdn-media-1.freecodecamp.org/imgr/eWWi3gZ.gif "offset")

## 21 - position: absolute;

- The next option for the CSS `position` property is `absolute`, which locks the element in place relative to its parent container. Unlike the `relative` position, this removes the element from the normal flow of the document, so surrounding items ignore it. The CSS offset properties (top or bottom and left or right) are used to adjust the position.

- One nuance with absolute positioning is that it will be locked relative to its closest positioned ancestor. If you forget to add a position rule to the parent item, (this is typically done using `position: relative;`), the browser will keep looking up the chain and ultimately default to the body tag.

## 22 - position: fixed :

- This is used to fix the element to the top or bottom while scrolling also it will be at given position.
- The next layout scheme that CSS offers is the `fixed` position, which is a type of absolute positioning that locks an element relative to the browser window. Similar to absolute positioning, it's used with the CSS offset properties and also removes the element from the normal flow of the document. Other items no longer "realize" where it is positioned, which may require some layout adjustments elsewhere.

- One key difference between the `fixed` and `absolute` positions is that an element with a fixed position won't move when the user scrolls.

## 23 - float :

- float is a positioning property which is used to keep the elements to float side by side like ballon.
- The next positioning tool does not actually use `position`, but sets the `float` property of an element. Floating elements are removed from the normal flow of a document and pushed to either the `left` or `right` of their containing parent element. It's commonly used with the `width` property to specify how much horizontal space the floated element requires.

## 24 - sticky :

- When elements are positioned to overlap (i.e. using `position: absolute | relative | fixed | sticky)`, the element coming later in the HTML markup will, by default, appear on the top of the other elements. However, the `z-index` property can specify the order of how elements are stacked on top of one another. It must be an integer (i.e. a whole number and not a decimal), and higher values for the `z-index` property of an element move it higher in the stack than those with lower values.

## 25 - margin :

- Another positioning technique is to center a block element horizontally. One way to do this is to set its `margin` to a value of auto.

- This method works for images, too. Images are inline elements by default, but can be changed to block elements when you set the `display` property to block.

## 26 - color theory :

- Color theory and its impact on design is a deep topic and only the basics are covered in the following challenges. On a website, color can draw attention to content, evoke emotions, or create visual harmony. Using different combinations of colors can really change the look of a website, and a lot of thought can go into picking a color palette that works with your content.

- The color wheel is a useful tool to visualize how colors relate to each other - it's a circle where similar hues are neighbors and different hues are farther apart. When two colors are opposite each other on the wheel, they are called complementary colors. They have the characteristic that if they are combined, they "cancel" each other out and create a gray color. However, when placed side-by-side, these colors appear more vibrant and produce a strong visual contrast.

- Some examples of complementary colors with their hex codes are:

```css
red (#FF0000) and cyan (#00FFFF)
green (#00FF00) and magenta (#FF00FF)
blue (#0000FF) and yellow (#FFFF00)
```

- This is different than the outdated RYB color model that many of us were taught in school, which has different primary and complementary colors. Modern color theory uses the additive RGB model (like on a computer screen) and the subtractive CMY(K) model (like in printing). Read here for more information on this complex subject.

There are many color picking tools available online that have an option to find the complement of a color.

Note: For all color challenges: Using color can be a powerful way to add visual interest to a page. However, color alone should not be used as the only way to convey important information because users with visual impairments may not understand that content. This issue will be covered in more detail in the Applied Accessibility challenges.
