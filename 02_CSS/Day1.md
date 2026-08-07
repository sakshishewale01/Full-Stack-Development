# Day 1: CSS Fundamentals

## 📌 Goal

The objective of Day 1 is to build a strong foundation in CSS by understanding how styles are applied to HTML elements. These concepts are essential for every Full Stack Developer and will be used in almost every web project.

---

# Topics Covered


1. Introduction to CSS
2. CSS Syntax
3. Types of CSS
4. CSS Selectors
5. Colors
6. Background
7. Fonts
8. Text Styling

---

# 1. Introduction to CSS

## What is CSS?

CSS (Cascading Style Sheets) is a stylesheet language used to describe the appearance and layout of HTML documents.

HTML creates the structure of a webpage, while CSS makes it visually attractive.

### Without CSS

- Plain webpage
- No colors
- No spacing
- No proper layout

### With CSS

- Beautiful colors
- Proper spacing
- Attractive fonts
- Responsive layouts
- Professional UI

### Why do we use CSS?

- Makes webpages attractive
- Separates design from content
- Improves user experience
- Allows code reusability
- Makes websites responsive

---

# 2. CSS Syntax

General Syntax

```css
selector {
    property: value;
}
```

Example

```css
h1 {
    color: blue;
}
```

### Parts of CSS Syntax

**Selector**

Selects the HTML element.

Example

```css
h1
```

**Property**

Defines what style should change.

Example

```css
color
```

**Value**

Specifies the value of the property.

Example

```css
blue
```

---

# 3. Types of CSS

## 1. Inline CSS

Applied directly inside an HTML element.

Example

```html
<h1 style="color:red;">Hello World</h1>
```

### Advantages

- Quick styling
- Good for testing

### Disadvantages

- Difficult to maintain
- Not reusable

---

## 2. Internal CSS

Written inside the `<style>` tag.

Example

```html
<head>

<style>

h1{
    color:blue;
}

</style>

</head>
```

### Advantages

- Good for single-page websites
- Easier than Inline CSS

### Disadvantages

- Cannot be reused across multiple pages

---

## 3. External CSS ⭐ (Most Important)

CSS is written in a separate `.css` file.

Example

```html
<link rel="stylesheet" href="style.css">
```

style.css

```css
h1{
    color:blue;
}
```

### Advantages

- Reusable
- Easy to maintain
- Professional approach
- Faster website loading due to browser caching

---

# CSS Priority

1. Inline CSS
2. Internal CSS
3. External CSS

---

# 4. CSS Selectors

Selectors tell CSS which HTML elements should receive the styles.

---

## Universal Selector

```css
*{
    margin:0;
}
```

Selects every element.

---

## Element Selector

```css
h1{
    color:red;
}
```

Selects all `<h1>` elements.

---

## Class Selector

HTML

```html
<p class="intro">Hello</p>
```

CSS

```css
.intro{
    color:green;
}
```

Selects elements having the same class.

---

## ID Selector

HTML

```html
<h1 id="title">CSS</h1>
```

CSS

```css
#title{
    color:blue;
}
```

Selects a unique element.

---

## Group Selector

```css
h1,p,button{
    color:black;
}
```

Applies the same style to multiple elements.

---

## Descendant Selector

```css
div p{
    color:red;
}
```

Selects `<p>` inside `<div>`.

---

# 5. Colors

Colors make webpages attractive.

### Ways to Apply Colors

### Color Name

```css
color:red;
```

---

### RGB

```css
color:rgb(255,0,0);
```

---

### RGBA

```css
color:rgba(255,0,0,0.5);
```

---

### HEX

```css
color:#ff0000;
```

---

### HSL

```css
color:hsl(0,100%,50%);
```

---

# Common Color Properties

```css
color
background-color
border-color
```

---

# 6. Background

Used to style the background of an element.

---

## Background Color

```css
background-color:skyblue;
```

---

## Background Image

```css
background-image:url("image.jpg");
```

---

## Background Repeat

```css
background-repeat:no-repeat;
```

---

## Background Size

```css
background-size:cover;
```

---

## Background Position

```css
background-position:center;
```

---

## Background Attachment

```css
background-attachment:fixed;

```

---

# 7. Fonts

Fonts improve readability.

---

## Font Family

```css
font-family:Arial,sans-serif;
```

---

## Font Size

```css
font-size:20px;
```

---

## Font Weight

```css
font-weight:bold;
```

---

## Font Style

```css
font-style:italic;
```

---

## Google Fonts

```html
<link href="https://fonts.googleapis.com/..." rel="stylesheet">
```

```css
font-family:'Poppins',sans-serif;
```

---

# 8. Text Styling

Text styling controls how text appears on the webpage.

---

## Color

```css
color:blue;
```

---

## Text Alignment

```css
text-align:center;
```

---

## Text Decoration

```css
text-decoration:none;
```

Common Values

- underline
- overline
- line-through
- none

---

## Text Transform

```css
text-transform:uppercase;
```

Values

- uppercase
- lowercase
- capitalize

---

## Letter Spacing

```css
letter-spacing:2px;
```

---

## Word Spacing

```css
word-spacing:5px;
```

---

## Line Height

```css
line-height:1.8;
```

---

## Text Shadow

```css
text-shadow:2px 2px 5px gray;
```

---

## Text Indent

```css
text-indent:40px;
```

---

## White Space

```css
white-space:nowrap;
```

---

# Mini Practice Project

Create a simple webpage containing:

- One Heading
- Two Paragraphs
- One Image
- One Button

Apply:

- Different Colors
- Background Color
- Font Family
- Font Size
- Text Alignment
- Text Decoration
- Text Transform

using an external CSS file.

---

# Interview Questions

### Q1. What is CSS?

CSS (Cascading Style Sheets) is a stylesheet language used to style and design HTML webpages.

---

### Q2. What are the three types of CSS?

- Inline CSS
- Internal CSS
- External CSS

---

### Q3. Which type of CSS is recommended?

External CSS because it is reusable, maintainable, and follows industry standards.

---

### Q4. What is a CSS Selector?

A selector is used to target HTML elements so that CSS styles can be applied to them.

---

### Q5. Difference between Class and ID?

| Class | ID |
|--------|----|
| Starts with `.` | Starts with `#` |
| Can be used multiple times | Should be unique |
| Reusable | Used for one specific element |

---

### Q6. Name different ways to specify colors in CSS.

- Color Name
- RGB
- RGBA
- HEX
- HSL

---

### Q7. What is the purpose of `text-decoration`?

It adds or removes decorations like underline, overline, line-through, or none.

---

### Q8. What is `font-family`?

It specifies the font used to display text.

---

# Day 1 Outcome

After completing Day 1, you will be able to:

- Understand the purpose of CSS
- Write CSS using correct syntax
- Apply Inline, Internal, and External CSS
- Use common CSS Selectors
- Apply colors and backgrounds
- Style fonts professionally
- Format text effectively
- Build and style a basic webpage using an external stylesheet

---

