# HTML Boilerplate

## 📖 What is an HTML Boilerplate?

An HTML boilerplate is the **basic structure** of every HTML document.

Every HTML page starts with this template, which tells the browser how to interpret and display the webpage.

Without this structure, browsers may not render the page correctly.

---

# Basic HTML Boilerplate

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>

</body>
</html>
```

---

# Explanation of Each Tag

## 1. `<!DOCTYPE html>`

### Purpose

Tells the browser that this document is written in **HTML5**.

Without it, browsers may enter **Quirks Mode**, which can display pages incorrectly.

---

## 2. `<html>`

This is the **root element** of every HTML page.

Everything inside the webpage must be placed between:

```html
<html>
...
</html>
```

---

## 3. `lang="en"`

Specifies the language of the webpage.

Example:

```html
<html lang="en">
```

Benefits:
- Helps search engines understand the page.
- Improves accessibility for screen readers.
- Assists browsers with language-specific features.

---

## 4. `<head>`

Contains information **about the webpage**, not the visible content.

Examples:
- Title
- Character encoding
- Stylesheets
- Metadata
- Icons

Content inside `<head>` is generally **not displayed** on the page.

---

## 5. `<meta charset="UTF-8">`(UTF- UNICODE Transformation Format)

Defines the character encoding.

UTF-8 supports:
- English
- Marathi
- Hindi
- Chinese
- Emojis 😊
- Most world languages

---

## 6. `<meta name="viewport">`

Makes the webpage responsive on different devices.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

Without this tag, a page may not display correctly on mobile devices.

---

## 7. `<title>`

Sets the title shown on the browser tab.

Example:

```html
<title>My Portfolio</title>
```

---

## 8. `<body>`

Contains everything visible on the webpage.

Examples:
- Headings
- Paragraphs
- Images
- Videos
- Tables
- Forms
- Buttons

---

# Browser Structure

HTML File

↓

Browser Reads HTML

↓

Interprets Tags

↓

Displays Webpage

---

# Best Practices

- Always include `<!DOCTYPE html>`.
- Set the correct language using `lang`.
- Include `UTF-8` character encoding.
- Add the viewport meta tag for responsiveness.
- Use meaningful page titles.

---

# Common Mistakes

❌ Forgetting `<!DOCTYPE html>`

❌ Missing `<title>`

❌ Placing visible content inside `<head>`

❌ Forgetting to close tags

---

# Interview Questions

### What is HTML Boilerplate?

The basic template required for every HTML document.

---

### Why do we use `<!DOCTYPE html>`?

To tell the browser that the document uses HTML5.

---

### What is the purpose of the `<head>` tag?

It stores metadata and resources related to the webpage.

---

### What is the purpose of the `<body>` tag?

It contains all the visible content displayed to the user.

---

# Summary

Every HTML page begins with a boilerplate.

Understanding each line helps create standards-compliant, accessible, and responsive web pages.