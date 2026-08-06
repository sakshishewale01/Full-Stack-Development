# HTML Tables

## 📖 Introduction

HTML tables are used to display data in rows and columns.

Tables are useful when information has a logical relationship between rows and columns.

Examples:

- Student Marks
- College Timetable
- Employee Records
- Product Comparison
- Cricket Scoreboard
- Invoice

---

# Basic Structure

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

---

# Table Tags

| Tag | Purpose |
|------|----------|
| `<table>` | Creates a table |
| `<tr>` | Table Row |
| `<th>` | Table Header |
| `<td>` | Table Data |
| `<caption>` | Table Title |
| `<thead>` | Header Section |
| `<tbody>` | Body Section |
| `<tfoot>` | Footer Section |

---

# 1. `<table>`

Container of the entire table.

Example

```html
<table>

</table>
```

---

# 2. `<tr>`

Creates one table row.

Example

```html
<tr>

</tr>
```

---

# 3. `<th>`

Creates a table heading.

Text inside `<th>` is bold and centered by default.

Example

```html
<th>Name</th>
```

---

# 4. `<td>`

Represents table data.

Example

```html
<td>Sakshi</td>
```

---

# 5. `<caption>`

Adds a title to the table.

Example

```html
<table>

<caption>
Student Details
</caption>

</table>
```

---

# Table Sections

## `<thead>`

Contains column headings.

## `<tbody>`

Contains main data.

## `<tfoot>`

Contains summary or footer information.

Example

```html
<table>

<thead>

<tr>

<th>Name</th>

<th>Marks</th>

</tr>

</thead>

<tbody>

<tr>

<td>Sakshi</td>

<td>95</td>

</tr>

</tbody>

<tfoot>

<tr>

<td>Total</td>

<td>95</td>

</tr>

</tfoot>

</table>
```

---

# colspan

Merges columns.

Example

```html
<td colspan="2">
Computer Engineering
</td>
```

---

# rowspan

Merges rows.

Example

```html
<td rowspan="2">
MITAOE
</td>
```

---

# Best Practices

- Always use `<th>` for headings.
- Use `<caption>` for accessibility.
- Organize tables using `<thead>`, `<tbody>`, and `<tfoot>`.
- Use tables only for tabular data.
- Do not use tables for webpage layout.

---

# Common Mistakes

❌ Using tables to design webpages.

❌ Forgetting `<th>`.

❌ Incorrect rowspan/colspan values.

❌ Missing `<caption>`.

---

# Interview Questions

### What is the purpose of `<table>`?

Creates a table.

---

### Difference between `<th>` and `<td>`?

`<th>` represents table headings.

`<td>` represents table data.

---

### What is `colspan`?

It merges multiple columns.

---

### What is `rowspan`?

It merges multiple rows.

---

### Why do we use `<thead>`, `<tbody>`, and `<tfoot>`?

To organize table content semantically and improve readability and accessibility.
<tfoot> is for footer section of a table.

---

# Summary

HTML tables organize related information into rows and columns.

Use semantic table sections and merge cells only when required.