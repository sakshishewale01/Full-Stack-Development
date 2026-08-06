# HTML Complete Cheat Sheet 🚀

Today's Date: 07/08/2026
Time: 12:26 am


A quick reference guide for all important HTML tags, their purpose, significance, syntax, and commonly used attributes.

---

# 1. HTML Boilerplate

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

### Purpose

Creates the basic structure of every HTML webpage.

### Significance

- Required for every HTML document.
- Helps browsers correctly render the webpage.

---

# 2. Heading Tags

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

### Purpose

Display headings from largest (`<h1>`) to smallest (`<h6>`).

### Significance

- Improves readability.
- Helps Search Engine Optimization (SEO).
- Creates a proper content hierarchy.

---

# 3. Paragraph

```html
<p>This is a paragraph.</p>
```

### Purpose

Displays text as a paragraph.

### Significance

Used for writing articles, descriptions, and content.

---

# 4. Line Break

```html
<br>
```

### Purpose

Moves content to the next line.

### Significance

Useful for addresses, poems, and formatted text.

---

# 5. Horizontal Rule

```html
<hr>
```

### Purpose

Creates a horizontal line.

### Significance

Separates different sections of a webpage.

---

# 6. Text Formatting Tags

| Tag | Purpose |
|------|---------|
| `<b>` | Bold text |
| `<strong>` | Important text (semantic) |
| `<i>` | Italic text |
| `<em>` | Emphasized text (semantic) |
| `<u>` | Underline text |
| `<mark>` | Highlight text |
| `<small>` | Smaller text |
| `<del>` | Deleted text |
| `<ins>` | Inserted text |
| `<sub>` | Subscript |
| `<sup>` | Superscript |

### Significance

Used to improve text presentation and meaning.

---

# 7. Anchor Tag

```html
<a href="https://github.com">GitHub</a>
```

### Purpose

Creates hyperlinks.

### Important Attributes

| Attribute | Purpose |
|-----------|---------|
| href | Destination URL |
| target="_blank" | Opens in new tab |
| title | Tooltip |
| download | Downloads file |

### Significance

Connects webpages and external resources.

---

# 8. Image Tag

```html
<img src="images/profile.jpg" alt="Profile" width="200">
```

### Purpose

Displays images.

### Important Attributes

| Attribute | Purpose |
|-----------|---------|
| src | Image path |
| alt | Alternative text |
| width | Image width |
| height | Image height |

### Significance

Makes webpages visually appealing and accessible.

---

# 9. Ordered List

```html
<ol>
    <li>HTML</li>
    <li>CSS</li>
</ol>
```

### Purpose

Creates numbered lists.

### Attributes

- type
- start
- reversed

---

# 10. Unordered List

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
</ul>
```

### Purpose

Creates bulleted lists.

---

# 11. Description List

```html
<dl>

    <dt>HTML</dt>

    <dd>HyperText Markup Language</dd>

</dl>
```

### Purpose

Displays terms with their descriptions.

### Tags

| Tag | Purpose |
|------|---------|
| `<dl>` | Description List |
| `<dt>` | Description Term |
| `<dd>` | Description Details |

### Significance

Useful for glossaries, FAQs, and dictionaries.

---

# 12. Tables

```html
<table>

    <tr>

        <th>Name</th>

        <th>Age</th>

    </tr>

    <tr>

        <td>Sakshi</td>

        <td>20</td>

    </tr>

</table>
```

### Purpose

Displays data in rows and columns.

### Important Tags

| Tag | Purpose |
|------|---------|
| `<table>` | Table container |
| `<tr>` | Table row |
| `<th>` | Table heading |
| `<td>` | Table data |
| `<caption>` | Table title |
| `<thead>` | Table header |
| `<tbody>` | Table body |
| `<tfoot>` | Table footer |

### Attributes

| Attribute | Purpose |
|-----------|---------|
| rowspan | Merge rows |
| colspan | Merge columns |

### Significance

Used for marksheets, invoices, schedules, reports, etc.

---

# 13. Forms

```html
<form>

</form>
```

### Purpose

Collects user input.

### Important Attributes

| Attribute | Purpose |
|-----------|---------|
| action | Destination URL |
| method | GET or POST |

---

# 14. Input Types

```html
<input type="text">
```

### Common Types

- text
- password
- email
- number
- tel
- date
- time
- color
- file
- radio
- checkbox
- submit
- reset

### Important Attributes

| Attribute | Purpose |
|-----------|---------|
| id | Unique identifier |
| name | Input name |
| value | Default value |
| placeholder | Hint text |
| required | Mandatory field |
| readonly | Read-only |
| disabled | Disable input |

---

# 15. Label

```html
<label for="name">Name</label>
```

### Purpose

Provides a label for input fields.

### Significance

Improves accessibility and user experience.

---

# 16. Textarea

```html
<textarea rows="5" cols="30"></textarea>
```

### Purpose

Accepts multi-line text.

### Significance

Used for comments, feedback, and addresses.

---

# 17. Select Dropdown

```html
<select>

    <option>Pune</option>

    <option>Mumbai</option>

</select>
```

### Purpose

Creates a dropdown menu.

---

# 18. Button

```html
<button>Click Me</button>
```

### Purpose

Creates clickable buttons.

### Types

- submit
- reset
- button

---

# 19. Audio

```html
<audio controls>

    <source src="audio/song.mp3" type="audio/mpeg">

</audio>
```

### Purpose

Embeds audio.

### Attributes

- controls
- autoplay
- loop
- muted

---

# 20. Video

```html
<video controls width="500">

    <source src="video/demo.mp4" type="video/mp4">

</video>
```

### Purpose

Embeds videos.

### Attributes

- controls
- autoplay
- muted
- loop
- poster
- width
- height

---

# 21. Iframe

```html
<iframe
src="https://www.youtube.com/embed/VIDEO_ID">
</iframe>
```

### Purpose

Embeds another webpage inside the current webpage.

### Uses

- YouTube Videos
- Google Maps
- PDFs
- External Websites

---

# 22. Semantic HTML

| Tag | Purpose |
|------|---------|
| `<header>` | Page header |
| `<nav>` | Navigation bar |
| `<main>` | Main content |
| `<section>` | Content section |
| `<article>` | Independent content |
| `<aside>` | Sidebar |
| `<footer>` | Footer |
| `<figure>` | Media container |
| `<figcaption>` | Caption for media |
| `<details>` | Expandable content |
| `<summary>` | Heading for details |

### Significance

- Better SEO
- Better Accessibility
- Cleaner Code
- Easier Maintenance

---

# HTML Best Practices

- Use semantic HTML whenever possible.
- Always include the `alt` attribute for images.
- Use `<label>` with form inputs.
- Use relative file paths.
- Maintain proper indentation.
- Use meaningful file and folder names.
- Avoid unnecessary `<br>` tags for spacing.
- Keep HTML clean and readable.

---

# HTML Folder Structure

```text
01_HTML/
│
├── 01_Introduction/
├── 02_Boilerplate/
├── 03_Headings_Paragraphs/
├── 04_Text_Formatting/
├── 05_Links/
├── 06_Images/
├── 07_Lists/
├── 08_Tables/
├── 09_Forms/
├── 10_Multimedia/
├── 11_Semantic_HTML/
└── README.md
```

---

# HTML Interview Tips

✅ Know the purpose of every HTML tag.

✅ Understand the difference between semantic and non-semantic HTML.

✅ Learn when to use lists, tables, and forms.

✅ Understand GET vs POST.

✅ Practice creating webpages without referring to notes.

✅ Focus on writing clean, semantic, and accessible HTML.
