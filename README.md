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

## 14 - font-size

- The font-size property is used to specify how large the text is in a given element. This rule can be used for multiple elements to create visual consistency of text on a page. In this challenge, you'll set the values for all h1 through h6 tags to balance the heading sizes.
