# Day 2: CSS Layout Fundamentals

## 📌 Goal

The objective of Day 2 is to understand the CSS properties responsible for spacing, sizing, layouts, and positioning. These concepts form the backbone of every modern website and are heavily used in Full Stack Development.

By the end of Day 2, you will be able to create structured, professional, and responsive webpage layouts.

---

# Topics Covered

1. Borders
2. Margin
3. Padding
4. Width & Height
5. CSS Box Model
6. Display Property
7. Flexbox

---

# 1. Borders

## What is Border?

A border is a line that surrounds an HTML element.

It is commonly used to highlight buttons, images, forms, cards, and containers.

---

## Border Syntax

```css
border: width style color;
```

Example

```css
border: 2px solid black;
```

---

## Border Width

```css
border-width: 3px;
```

---

## Border Style

```css
border-style: solid;
```

Common Values

- solid
- dotted
- dashed
- double
- groove
- ridge
- inset
- outset
- none

---

## Border Color

```css
border-color: red;
```

---

## Border Radius

Creates rounded corners.

```css
border-radius: 10px;
```

For a perfect circle:

```css
border-radius: 50%;
```

---

## Individual Borders

```css
border-top: 2px solid red;

border-right: 2px solid blue;

border-bottom: 2px solid green;

border-left: 2px solid orange;
```

---

# 2. Margin

## What is Margin?

Margin is the space outside an element.

It creates distance between neighboring elements.

---

Example

```css
margin: 20px;
```

---

## Individual Margins

```css
margin-top: 20px;

margin-right: 15px;

margin-bottom: 20px;

margin-left: 15px;
```

---

## Shorthand

```css
margin: 20px;
```

All sides

```css
margin: 20px 30px;
```

Top-Bottom Left-Right

```css
margin: 20px 30px 10px;
```

Top Left-Right Bottom

```css
margin: 10px 20px 30px 40px;
```

Top Right Bottom Left

---

## Centering an Element

```css
margin: auto;
```

Used with a specified width.

Example

```css
width: 300px;

margin: auto;
```

---

# 3. Padding

## What is Padding?

Padding is the space inside an element between the content and its border.

---

Example

```css
padding: 20px;
```

---

## Individual Padding

```css
padding-top: 10px;

padding-right: 20px;

padding-bottom: 10px;

padding-left: 20px;
```

---

## Shorthand

```css
padding: 20px;

padding: 20px 30px;

padding: 20px 30px 10px;

padding: 10px 20px 30px 40px;
```

---

# Margin vs Padding

| Margin | Padding |
|---------|----------|
| Outside the border | Inside the border |
| Creates space between elements | Creates space inside an element |
| Background color does not apply | Background color extends into padding |

---

# 4. Width & Height

Used to define the size of elements.

---

## Width

```css
width: 300px;
```

---

## Height

```css
height: 200px;
```

---

## Maximum Width

```css
max-width: 600px;
```

---

## Minimum Width

```css
min-width: 250px;
```

---

## Maximum Height

```css
max-height: 400px;
```

---

## Minimum Height

```css
min-height: 100px;
```

---

# Common Units

| Unit | Description |
|-------|-------------|
| px | Pixels |
| % | Percentage |
| rem | Relative to root font size |
| em | Relative to parent font size |
| vw | Viewport width |
| vh | Viewport height |

---

# 5. CSS Box Model ⭐⭐⭐⭐⭐

## What is Box Model?

Every HTML element is treated as a rectangular box.

The Box Model consists of four parts:

```text
Margin

↓

Border

↓

Padding

↓

Content
```

Visual Representation

```text
+---------------------------+
|         Margin            |
|  +---------------------+  |
|  |      Border         |  |
|  |  +---------------+  |  |
|  |  |   Padding     |  |  |
|  |  | +-----------+ |  |  |
|  |  | | Content   | |  |  |
|  |  | +-----------+ |  |  |
|  |  +---------------+  |  |
|  +---------------------+  |
+---------------------------+
```

---

## Example

```css
div{

width:300px;

padding:20px;

border:5px solid black;

margin:30px;

}
```

---

## Box Sizing

### Content Box (Default)

```css
box-sizing: content-box;
```

---

### Border Box (Recommended)

```css
box-sizing: border-box;
```

This includes padding and border inside the specified width.

Most developers use:

```css
*{

box-sizing:border-box;

}
```

---

# 6. Display Property

Controls how elements are displayed.

---

## Block Elements

Take full width.

Examples

- div
- h1
- p
- section

Example

```css
display:block;
```

---

## Inline Elements

Take only required width.

Examples

- span
- a
- strong
- em

Example

```css
display:inline;
```

---

## Inline-Block

Acts like inline but accepts width and height.

```css
display:inline-block;
```

---

## None

Hides the element.

```css
display:none;
```

---

# Display Comparison

| Property | New Line | Width/Height |
|----------|----------|--------------|
| block | Yes | Yes |
| inline | No | No |
| inline-block | No | Yes |
| none | Hidden | Hidden |

---

# 7. Flexbox ⭐⭐⭐⭐⭐

## What is Flexbox?

Flexbox is a one-dimensional layout system used to arrange items horizontally or vertically.

It is the most commonly used layout method in modern web development.

---

## Enable Flexbox

```css
display:flex;
```

---

## Flex Direction

```css
flex-direction:row;
```

Default

```css
flex-direction:column;
```

---

## Justify Content

Controls horizontal alignment.

```css
justify-content:center;
```

Common Values

- flex-start
- center
- flex-end
- space-between
- space-around
- space-evenly

---

## Align Items

Controls vertical alignment.

```css
align-items:center;
```

Common Values

- stretch
- center
- flex-start
- flex-end

---

## Gap

Creates spacing between flex items.

```css
gap:20px;
```

---

## Flex Wrap

Allows items to move to the next line.

```css
flex-wrap:wrap;
```

---

## Example

```css
.container{

display:flex;

justify-content:space-between;

align-items:center;

gap:20px;

}
```

---

# Mini Practice Project

Create a webpage containing:

- Header
- Navigation Bar
- Three Cards
- Footer

Apply

- Border
- Border Radius
- Margin
- Padding
- Width
- Height
- Box Model
- Display
- Flexbox

---

# Interview Questions

## Q1. What is the difference between Margin and Padding?

Margin creates space outside an element.

Padding creates space inside an element between the content and border.

---

## Q2. What is the CSS Box Model?

The Box Model consists of:

- Content
- Padding
- Border
- Margin

Every HTML element follows this structure.

---

## Q3. What is `box-sizing: border-box`?

It includes padding and border inside the specified width and height of an element.

It makes layout calculations easier.

---

## Q4. Difference between Block and Inline elements?

| Block | Inline |
|--------|---------|
| Takes full width | Takes only required width |
| Starts on new line | Does not start on new line |
| Width and Height work | Width and Height generally do not work |

---

## Q5. What is Flexbox?

Flexbox is a CSS layout model used to arrange elements efficiently in one direction (row or column).

---

## Q6. What is the default value of `flex-direction`?

```css
row
```

---

## Q7. What is the purpose of `justify-content`?

It aligns flex items along the main axis (usually horizontal).

---

## Q8. What is the purpose of `align-items`?

It aligns flex items along the cross axis (usually vertical).

---

## Q9. What is the purpose of `display: none`?

It completely hides the element from the webpage.

---

## Day 2 Outcome

After completing Day 2, you will be able to:

- Add borders to elements
- Create spacing using margin and padding
- Control element size using width and height
- Understand and apply the CSS Box Model
- Use different display properties
- Build layouts using Flexbox
- Design clean and professional webpage structures

---

# Next Step (Day 3)

Topics Covered:

- Position
- CSS Grid (Basics)
- Responsive Design
- Media Queries
- Hover Effects
- Cursor
- Opacity
- Box Shadow
- Transitions
- CSS Transform (Basics)
- Final CSS Projects