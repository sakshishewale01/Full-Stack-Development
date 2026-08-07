# Day 3: Responsive Design & Modern CSS

## 📌 Goal

The objective of Day 3 is to learn the CSS concepts used to build modern, responsive, and interactive websites. These topics are widely used in React, Angular, Next.js, and other frontend frameworks.

By the end of Day 3, you will be able to build responsive webpages that look good on desktops, tablets, and mobile devices.

---

# Topics Covered

1. Position
2. CSS Grid (Basics)
3. Responsive Design
4. Media Queries
5. Cursor
6. Opacity
7. Box Shadow
8. Hover Effects
9. Transitions
10. CSS Transform (Basics)

---

# 1. Position

## What is Position?

The `position` property specifies how an HTML element is positioned on a webpage.

---

## Types of Position

### Static (Default)

The default positioning of every HTML element.

```css
position: static;
```

---

### Relative

Moves the element relative to its original position.

```css
position: relative;

top:20px;

left:30px;
```

---

### Absolute

Positions an element relative to its nearest positioned parent.

```css
position:absolute;

top:20px;

right:20px;
```

---

### Fixed

The element stays fixed even while scrolling.

Used for:

- Navigation Bars
- Chat Buttons
- Back to Top Button

```css
position:fixed;

bottom:20px;

right:20px;
```

---

### Sticky

Acts like Relative until scrolling reaches a specific point.

Then behaves like Fixed.

```css
position:sticky;

top:0;
```

Used for

- Sticky Navigation Bars
- Sticky Headers

---

# Position Comparison

| Position | Scrolls? | Relative To |
|----------|----------|-------------|
| Static | Yes | Normal Flow |
| Relative | Yes | Original Position |
| Absolute | Yes | Parent Element |
| Fixed | No | Browser Window |
| Sticky | Partially | Scroll Position |

---

# 2. CSS Grid (Basics)

## What is Grid?

CSS Grid is a two-dimensional layout system.

Flexbox works in one direction.

Grid works in rows and columns.

---

## Enable Grid

```css
display:grid;
```

---

## Create Columns

```css
grid-template-columns:1fr 1fr 1fr;
```

Three equal columns

---

## Gap

```css
gap:20px;
```

---

## Example

```css
.container{

display:grid;

grid-template-columns:repeat(3,1fr);

gap:20px;

}
```

---

## Why Grid?

Used for

- Dashboards
- Gallery Layouts
- Admin Panels
- Cards

---

# Flexbox vs Grid

| Flexbox | Grid |
|----------|------|
| One Direction | Two Directions |
| Row OR Column | Rows AND Columns |
| Navigation Bars | Complete Layouts |

---

# 3. Responsive Design

## What is Responsive Design?

Responsive Design means a webpage automatically adjusts its layout according to the device size.

It should work properly on

- Desktop
- Laptop
- Tablet
- Mobile

---

## Importance

Without Responsive Design

❌ Website breaks on mobile.

With Responsive Design

✅ Website looks good on every device.

---

# Responsive Units

Instead of always using pixels,

learn

```css
%

rem

em

vw

vh
```

---

# Images

Responsive Images

```css
img{

max-width:100%;

height:auto;

}
```

---

# Containers

```css
width:90%;

max-width:1200px;

margin:auto;
```

---

# 4. Media Queries

## What are Media Queries?

Media Queries apply different CSS styles for different screen sizes.

---

## Syntax

```css
@media(max-width:768px){

body{

background:lightblue;

}

}
```

---

## Common Breakpoints

### Mobile

```css
@media(max-width:576px)
```

---

### Tablet

```css
@media(max-width:768px)
```

---

### Laptop

```css
@media(max-width:992px)
```

---

### Desktop

```css
@media(min-width:1200px)
```

---

## Example

```css
.container{

display:flex;

}

@media(max-width:768px){

.container{

flex-direction:column;

}

}
```

---

# 5. Cursor

Changes the mouse cursor.

---

Example

```css
cursor:pointer;
```

---

Common Values

```css
pointer

default

move

text

wait

help

not-allowed
```

---

# 6. Opacity

Controls transparency.

Range

```
0 → Invisible

1 → Fully Visible
```

Example

```css
opacity:0.5;
```

---

# 7. Box Shadow

Adds shadow around an element.

---

Syntax

```css
box-shadow:

horizontal

vertical

blur

color;
```

Example

```css
box-shadow:5px 5px 15px gray;
```

---

Cards

Buttons

Forms

Navigation Bars

commonly use Box Shadow.

---

# 8. Hover Effects

Hover changes an element's appearance when the mouse is placed over it.

Example

```css
button:hover{

background:blue;

color:white;

}
```

Hover is heavily used in

- Buttons
- Links
- Cards
- Images

---

# 9. Transitions

Transitions create smooth animations.

Without Transition

Instant Change

With Transition

Smooth Change

---

Syntax

```css
transition:0.5s;
```

Example

```css
button{

background:red;

transition:0.3s;

}

button:hover{

background:green;

}
```

---

# Transition Properties

```css
transition-property

transition-duration

transition-delay

transition-timing-function
```

---

# 10. CSS Transform (Basics)

Transforms change the appearance of elements.

---

## Scale

```css
transform:scale(1.1);
```

Makes element larger.

---

## Rotate

```css
transform:rotate(10deg);
```

---

## Translate

```css
transform:translateX(20px);
```

---

## Skew

```css
transform:skew(10deg);
```

---

## Example

```css
.card:hover{

transform:scale(1.05);

}
```

---

# Mini Practice Project

Build a webpage containing

- Navigation Bar
- Hero Section
- Three Cards
- Gallery
- Footer

Apply

- Position
- Grid
- Media Queries
- Hover
- Transition
- Box Shadow
- Transform

---

# Interview Questions

## Q1. Difference between Relative and Absolute Position?

Relative moves relative to itself.

Absolute moves relative to its positioned parent.

---

## Q2. Difference between Fixed and Sticky?

Fixed always stays at one position.

Sticky becomes fixed only after reaching a certain scroll position.

---

## Q3. Difference between Grid and Flexbox?

Flexbox is one-dimensional.

Grid is two-dimensional.

---

## Q4. What is Responsive Design?

Responsive Design ensures that webpages automatically adjust according to different screen sizes.

---

## Q5. What are Media Queries?

Media Queries allow developers to apply different CSS rules depending on the device width or height.

---

## Q6. What is the use of Box Shadow?

Adds shadow effects around elements.

---

## Q7. What is Hover?

Hover changes an element's appearance when the mouse pointer is placed over it.

---

## Q8. What is Transition?

Transition creates smooth changes between CSS property values.

---

## Q9. Difference between Opacity and Visibility?

Opacity makes an element transparent while still occupying space.

Visibility hides an element but still reserves its layout space.

---

## Q10. What is Transform?

Transform modifies the appearance of an element by scaling, rotating, translating, or skewing it.

---

# Day 3 Outcome

After completing Day 3, you will be able to:

- Position elements accurately using different positioning techniques.
- Build layouts using CSS Grid.
- Design responsive webpages for different devices.
- Use Media Queries to adapt layouts.
- Apply cursor styles for better user experience.
- Create transparent effects using opacity.
- Add professional shadows using Box Shadow.
- Design interactive hover effects.
- Create smooth animations with transitions.
- Transform elements using scale, rotate, translate, and skew.

---

# 🎉 Congratulations!

You have successfully completed the CSS roadmap required for Full Stack Development.

You now know:

- ✅ CSS Fundamentals
- ✅ Colors & Backgrounds
- ✅ Fonts & Text Styling
- ✅ Borders, Margin & Padding
- ✅ Box Model
- ✅ Display
- ✅ Flexbox
- ✅ Position
- ✅ CSS Grid
- ✅ Responsive Design
- ✅ Media Queries
- ✅ Hover Effects
- ✅ Box Shadow
- ✅ Transitions
- ✅ Basic Transforms

---

# 🚀 What's Next?

Now it's time to apply everything you've learned by building **three CSS projects**.

### Project 1: Personal Profile Website
**Concepts Covered:**
- Colors
- Fonts
- Margin & Padding
- Borders
- Border Radius
- Box Shadow
- Hover Effects

### Project 2: Restaurant Website
**Concepts Covered:**
- Flexbox
- Grid
- Navigation Bar
- Cards
- Responsive Layout
- Image Styling
- Hover Effects
- Media Queries

### Project 3: Student Registration Form
**Concepts Covered:**
- Form Styling
- Responsive Design
- Buttons
- Input Fields
- Shadows
- Transitions
- Focus Effects

These three projects will prepare you well before moving on to **JavaScript**, where you'll begin adding real interactivity to your websites.