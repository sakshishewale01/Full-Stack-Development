# HTML Lists

## 📖 Introduction

HTML provides different types of lists to organize information in a structured and readable format.

Lists improve readability and help users quickly understand grouped information.

---

# Types of Lists

HTML supports three types of lists:

1. Ordered List (`<ol>`)
2. Unordered List (`<ul>`)
3. Description List (`<dl>`)

---

# 1. Ordered List

An ordered list displays items in a numbered sequence.

Syntax

```html
<ol>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ol>
```

Output

1. HTML
2. CSS
3. JavaScript

---

# Ordered List Attributes

## type

Changes the numbering style.

```html
<ol type="A">
```

Possible values

| Value | Output |
|--------|---------|
| 1 | 1,2,3 |
| A | A,B,C |
| a | a,b,c |
| I | I,II,III |
| i | i,ii,iii |

---

## start

Starts numbering from a specific value.

```html
<ol start="5">
```

Output

5. Item
6. Item

---

## reversed

Displays numbering in reverse order.

```html
<ol reversed>
```

Output

3
2
1

---

# 2. Unordered List

Displays bullet points.

Syntax

```html
<ul>

    <li>Apple</li>

    <li>Mango</li>

    <li>Orange</li>

</ul>
```

---

# Bullet Styles

Using CSS is the modern approach, but HTML supports:

```html
<ul type="circle">
```

Options

- disc
- circle
- square

---

# 3. Description List

Used for definitions or terms.

Syntax

```html
<dl>

<dt>HTML</dt>

<dd>Markup Language</dd>

<dt>CSS</dt>

<dd>Styling Language</dd>

</dl>
```

---

# Nested Lists

Lists can contain other lists.

Example

```html
<ul>

<li>

Programming

<ul>

<li>Java</li>

<li>Python</li>

</ul>

</li>

</ul>
```

---

# Real-World Uses

- Website Navigation
- Restaurant Menu
- Product Features
- Resume Skills
- Shopping Lists
- Documentation
- FAQs

---

# Best Practices

- Use ordered lists when sequence matters.
- Use unordered lists when order does not matter.
- Use description lists for terms and definitions.
- Keep nesting meaningful.
- Write clear list items.

---

# Common Mistakes

❌ Using `<br>` instead of lists.

❌ Forgetting `<li>`.

❌ Using ordered lists when order doesn't matter.

❌ Deeply nested lists that are hard to read.

---

# Interview Questions

### What are the three types of HTML lists?

- Ordered List
- Unordered List
- Description List

---

### Difference between `<ol>` and `<ul>`?

`<ol>` displays numbered items.

`<ul>` displays bullet points.

---

### What is `<li>`?

Defines an individual list item.

---

### What is `<dl>`?

A description list used for terms and definitions.

---

### What is a nested list?

A list placed inside another list.

### What is the purpose of <dl>, <dt>, and <dd>?

<dl> is used to create a description (definition) list. Inside it, <dt> defines the term or title, and <dd> provides the description or details of that term. It is commonly used for glossaries, FAQs, technical documentation, and dictionaries.
---

# Summary

HTML lists organize content in a structured manner.

Choose the correct list type depending on whether order matters, bullets are sufficient, or definitions are required.