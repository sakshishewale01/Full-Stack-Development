# Semantic HTML

## 📖 Introduction

Semantic HTML uses meaningful HTML elements that clearly describe the purpose of the content.

Instead of writing:

```html
<div>
```

We can use:

```html
<header>
<nav>
<main>
<section>
<article>
<aside>
<footer>
```

This makes code easier to read for developers, browsers, search engines, and screen readers.

---

# Why Semantic HTML?

Benefits:

- Better code readability
- Improved SEO
- Better accessibility
- Easier maintenance
- Professional coding practices

---

# Common Semantic Tags

| Tag | Purpose |
|------|----------|
| `<header>` | Header of a page or section |
| `<nav>` | Navigation links |
| `<main>` | Main content |
| `<section>` | A section of content |
| `<article>` | Independent content |
| `<aside>` | Sidebar or related information |
| `<footer>` | Footer section |
| `<figure>` | Groups media content |
| `<figcaption>` | Caption for media |
| `<details>` | Expandable content |
| `<summary>` | Heading for `<details>` |

---

# `<header>`

Represents the introductory content.

Example

```html
<header>
    <h1>My Portfolio</h1>
</header>
```

---

# `<nav>`

Contains navigation links.

```html
<nav>

<a href="#">Home</a>

<a href="#">About</a>

<a href="#">Projects</a>

</nav>
```

---

# `<main>`

Contains the primary content of the webpage.

```html
<main>

</main>
```

Only one `<main>` should exist on a page.

---

# `<section>`

Represents a logical section.

Example

```html
<section>

<h2>Skills</h2>

<p>HTML CSS JavaScript</p>

</section>
```

---

# `<article>`

Represents independent content.

Examples:

- Blog post
- News article
- Product card

```html
<article>

<h2>My First Blog</h2>

<p>Content...</p>

</article>
```

---

# `<aside>`

Contains related information.

Examples:

- Sidebar
- Recent Posts
- Advertisements

---

# `<footer>`

Represents footer information.

```html
<footer>

<p>© 2026 Sakshi Shewale</p>

</footer>
```

---

# `<figure>` and `<figcaption>`

```html
<figure>

<img src="profile.jpg"
alt="Profile">

<figcaption>
My Profile Picture
</figcaption>

</figure>
```

---

# `<details>` and `<summary>`

Creates expandable content.

```html
<details>

<summary>
Click Here
</summary>

<p>
Hidden information
</p>

</details>
```

---

# Semantic vs Non-Semantic

Non-Semantic

```html
<div>
<div>
<div>
```

Semantic

```html
<header>
<nav>
<main>
<section>
<footer>
```

---

# Best Practices

- Use semantic tags whenever possible.
- Only one `<main>` element.
- Use `<article>` for independent content.
- Use `<section>` for grouped content.
- Avoid unnecessary `<div>` elements.

---

# Common Mistakes

❌ Using `<div>` everywhere.

❌ Multiple `<main>` elements.

❌ Using `<section>` without a heading.

---

# Interview Questions

### What is Semantic HTML?

HTML that uses meaningful tags describing content.

---

### Difference between `<section>` and `<article>`?

`<section>` groups related content.

`<article>` is self-contained and can stand alone.

---

### Why use Semantic HTML?

Better SEO, accessibility, readability, and maintainability.

---

# Summary

Semantic HTML creates cleaner, more meaningful webpages using tags that describe their content instead of generic containers.