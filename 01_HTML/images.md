# HTML Images (`<img>` Tag)

## 📖 Introduction

The `<img>` tag is used to display images on a webpage.

Unlike most HTML tags, `<img>` is a **void (self-closing) element**, which means it does not require a closing tag.

Images improve the visual appearance of a website and help communicate information more effectively.

---

# Syntax

```html
<img src="image.jpg" alt="Description">
```

---

# Anatomy of the `<img>` Tag

```html
<img src="profile.jpg" alt="Profile Photo" width="250">
```

| Attribute | Purpose |
|-----------|---------|
| `src` | Specifies the image path |
| `alt` | Alternative text if the image cannot load |
| `width` | Sets image width |
| `height` | Sets image height |

---

# Image Sources

## 1. Relative Path

Used when the image is inside your project.

```html
<img src="images/profile.jpg" alt="Profile">
```

---

## 2. Absolute URL

Used when the image is hosted on another website.

```html
<img src="https://example.com/logo.png" alt="Logo">
```

---

# Why is `alt` Important?

The `alt` attribute:

- Improves accessibility for screen readers.
- Displays text if the image cannot be loaded.
- Helps search engines understand the image.

Example:

```html
<img src="student.jpg" alt="Student studying on a laptop">
```

---

# Image Formats

## JPEG (.jpg / .jpeg)

- Best for photographs
- Smaller file size
- Supports millions of colors

---

## PNG (.png)

- Supports transparent backgrounds
- Good for logos and graphics

---

## SVG (.svg)

- Vector format
- Scales without losing quality
- Best for icons and logos

---

## WebP (.webp)

- Modern image format
- Better compression
- High quality with smaller file size

---

## GIF (.gif)

- Supports simple animations

---

# Width and Height

```html
<img src="profile.jpg"
     width="250"
     height="250"
     alt="Profile">
```

---

# Figure and Figcaption

```html
<figure>

    <img src="college.jpg"
         alt="College Campus">

    <figcaption>
        MIT Academy of Engineering
    </figcaption>

</figure>
```

Use `<figure>` to group an image with its caption.

---

# Best Practices

- Always provide an `alt` attribute.
- Use appropriate image formats.
- Keep image file sizes small.
- Organize images inside an `images/` folder.
- Use meaningful filenames.

---

# Common Mistakes

❌ Missing `alt`

❌ Very large image files

❌ Incorrect file paths

❌ Using spaces in filenames

---

# Interview Questions

### What is the purpose of the `<img>` tag?

To display images on a webpage.

---

### What is the `src` attribute?

It specifies the location of the image.

---

### Why do we use `alt`?

For accessibility and as fallback text if the image cannot load.

---

### Difference between JPEG and PNG?

JPEG is better for photographs.

PNG supports transparency.

---

### What is SVG?

A vector image format that scales without losing quality.

---

# Summary

The `<img>` tag is essential for displaying images. Using the correct image format, proper file paths, and meaningful `alt` text creates accessible and professional webpages.