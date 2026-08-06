# HTML Text Formatting

## 📖 Introduction

HTML provides several tags to format text. These tags help emphasize important content, display mathematical formulas, write code snippets, highlight text, and improve accessibility.

Formatting tags not only change the appearance of text but also provide meaning to browsers, search engines, and assistive technologies.

---

# 1. Bold Text

## `<b>`

Makes text bold without adding semantic importance.

Example

```html
<b>This is bold text.</b>
```

Use when the text should simply appear bold.

---

# 2. Strong Text

## `<strong>`

Indicates that the content is important.

Example

```html
<strong>This is important.</strong>
```

Browsers display it in bold, but it also carries semantic meaning.

---

# Difference

| `<b>` | `<strong>` |
|--------|------------|
| Visual formatting | Semantic importance |
| Bold only | Important content |

---

# 3. Italic Text

## `<i>`

Displays text in italics.

Example

```html
<i>Harry Potter</i>
```

Often used for book titles, foreign words, or technical terms.

---

# 4. Emphasized Text

## `<em>`

Adds emphasis to text.

Example

```html
<em>Read this carefully.</em>
```

Browsers usually display it in italics, but it also adds meaning.

---

# Difference

| `<i>` | `<em>` |
|--------|---------|
| Italic styling | Semantic emphasis |

---

# 5. Underline

```html
<u>Underlined Text</u>
```

---

# 6. Highlight

```html
<mark>Highlighted Text</mark>
```

Used to highlight important information.

---

# 7. Small Text

```html
<small>Terms and Conditions Apply</small>
```

Displays smaller-sized text.

---

# 8. Deleted Text

```html
<del>₹999</del>
```

Represents deleted or removed content.

---

# 9. Inserted Text

```html
<ins>₹799</ins>
```

Represents newly inserted content.

---

# 10. Subscript

```html
H<sub>2</sub>O
```

Used in chemical formulas.

---

# 11. Superscript

```html
x<sup>2</sup>
```

Used in mathematical expressions.

---

# 12. Code

```html
<code>System.out.println("Hello");</code>
```

Displays programming code.

---

# 13. Preformatted Text

```html
<pre>
Name : Sakshi
Age  : 20
City : Pune
</pre>
```

Preserves spaces and line breaks exactly as written.

---

# Best Practices

- Use `<strong>` instead of `<b>` when the content is important.
- Use `<em>` instead of `<i>` when emphasizing text.
- Use `<mark>` only for important highlights.
- Use `<code>` for code snippets.
- Use `<pre>` for preserving formatting.

---

# Common Mistakes

❌ Using `<b>` everywhere instead of `<strong>`.

❌ Using `<br>` instead of `<pre>` for formatted text.

❌ Forgetting to close formatting tags.

---

# Interview Questions

### Difference between `<b>` and `<strong>`?

`<b>` only changes appearance.

`<strong>` adds semantic importance.

---

### Difference between `<i>` and `<em>`?

`<i>` changes appearance.

`<em>` adds emphasis.

---

### Why use `<code>`?

To display programming code.

---

### Why use `<pre>`?

To preserve spaces and line breaks.

---

# Summary

Formatting tags improve readability, accessibility, and semantic meaning while helping organize different kinds of text effectively.