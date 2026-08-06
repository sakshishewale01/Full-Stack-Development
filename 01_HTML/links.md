# HTML Links (`<a>` Tag)

## 📖 Introduction

The `<a>` (anchor) tag is used to create hyperlinks in HTML.

Hyperlinks connect one webpage to another, allowing users to navigate between pages, websites, documents, email addresses, phone numbers, and specific sections within a webpage.

Without hyperlinks, the World Wide Web would not function as we know it.

---

# Syntax

```html
<a href="URL">Link Text</a>
```

Example

```html
<a href="https://www.google.com">Visit Google</a>
```

---

# Anatomy of an Anchor Tag

```html
<a href="https://www.google.com">Google</a>
```

| Part | Meaning |
|------|---------|
| `<a>` | Anchor tag |
| `href` | Hypertext Reference (destination URL) |
| `Google` | Clickable text |
| `</a>` | Closing tag |

---

# Types of Links

## 1. External Link

Links to another website.

```html
<a href="https://www.google.com">
Google
</a>
```

---

## 2. Internal Link

Links to another page within the same project.

```html
<a href="about.html">
About Us
</a>
```

---

## 3. Email Link

Opens the default email application.

```html
<a href="mailto:sakshi@example.com">
Send Email
</a>
```

---

## 4. Phone Link

Useful for mobile devices.

```html
<a href="tel:+919876543210">
Call Now
</a>
```

---

## 5. Open Link in New Tab

```html
<a href="https://github.com"
   target="_blank">
GitHub
</a>
```

### Why use `target="_blank"`?

It opens the destination in a new browser tab while keeping the current page open.

---

## 6. Download Link

```html
<a href="resume.pdf" download>
Download Resume
</a>
```

Downloads the file instead of opening it.

---

## 7. Image as a Link

```html
<a href="https://www.google.com">

<img src="logo.png" width="100">

</a>
```

Clicking the image opens the link.

---

## 8. Bookmark (Jump to Section)

```html
<a href="#contact">
Go to Contact
</a>
```

Destination

```html
<h2 id="contact">
Contact
</h2>
```

---

# Absolute vs Relative URL

## Absolute URL

Contains the complete website address.

```html
https://github.com
```

---

## Relative URL

Points to another file inside the same project.

```html
about.html
```

---

# Important Attributes

## href

Specifies the destination.

---

## target

Specifies where the page opens.

Examples

```html
target="_self"
```

Default

Opens in same tab.

```html
target="_blank"
```

Opens in new tab.

---

## title

Shows a tooltip.

```html
<a href="about.html"
title="About Us">

About

</a>
```

---

# Best Practices

- Use meaningful link text.
- Avoid "Click Here".
- Use `target="_blank"` only when appropriate.
- Check that links are not broken.
- Use descriptive titles.

---

# Common Mistakes

❌ Missing `href`

❌ Broken links

❌ Using spaces in filenames

❌ Forgetting closing tag

---

# Interview Questions

### What is the purpose of the `<a>` tag?

Creates hyperlinks between webpages.

---

### What is `href`?

Specifies the destination URL.

---

### Difference between Absolute and Relative URL?

Absolute contains the complete website address.

Relative points to files inside the same project.

---

### What is `target="_blank"`?

Opens the webpage in a new browser tab.

---

### Difference between Internal and External Links?

Internal links connect pages within the same website.

External links connect to different websites.

---

# Summary

The `<a>` tag is one of the most important HTML elements.

It enables navigation between pages, websites, documents, email addresses, phone numbers, and webpage sections.