# HTML Forms

## 📖 Introduction

HTML forms are used to collect information from users.

Forms allow users to enter data, which can then be sent to a server for processing.

Examples:

- Login Page
- Registration Form
- Contact Form
- College Admission Form
- Feedback Form
- Search Bar

---

# Basic Syntax

```html
<form>

</form>
```

Everything related to user input is placed inside the `<form>` element.

---

# Form Attributes

## action

Specifies where the form data is sent.

```html
<form action="/submit">
```

---

## method

Specifies how the data is sent.

```html
<form method="GET">
```

or

```html
<form method="POST">
```

### GET

- Sends data through the URL.
- Suitable for search forms.

### POST

- Sends data in the request body.
- Suitable for passwords and sensitive data.

---

# Input Element

```html
<input>
```

Used to collect information from users.

---

# Common Input Types

| Type | Purpose |
|------|---------|
| text | Single-line text |
| password | Password |
| email | Email address |
| number | Numeric value |
| tel | Phone number |
| date | Date selection |
| time | Time selection |
| color | Color picker |
| file | Upload files |
| checkbox | Multiple selections |
| radio | Single selection |
| submit | Submit form |
| reset | Reset form |

---

# Label

```html
<label>Name</label>
```

Provides a description for an input field.

Better accessibility:

```html
<label for="name">Name</label>

<input
id="name"
type="text">
```

---

# Placeholder

```html
<input
type="text"
placeholder="Enter your name">
```

Displays a hint inside the input box.

---

# Required

```html
<input
type="email"
required>
```

Makes the field mandatory.

---

# Radio Button

Allows only one selection.

```html
<input
type="radio"
name="gender">

Male
```

All radio buttons in the same group must have the same `name`.

---

# Checkbox

Allows multiple selections.

```html
<input
type="checkbox">

HTML
```

---

# Textarea

Used for long text.

```html
<textarea
rows="5"
cols="30">

</textarea>
```

---

# Select Dropdown

```html
<select>

<option>Pune</option>

<option>Mumbai</option>

<option>Nashik</option>

</select>
```

---

# Buttons

Submit

```html
<input
type="submit">
```

Reset

```html
<input
type="reset">
```

Button

```html
<button>
Click Me
</button>
```

---

# Best Practices

- Always use labels.
- Use meaningful placeholders.
- Mark required fields.
- Group related radio buttons.
- Validate user input.
- Keep forms simple.

---

# Common Mistakes

❌ Missing labels.

❌ Using GET for passwords.

❌ Forgetting the `name` attribute.

❌ Using radio buttons without a common `name`.

---

# Interview Questions

### What is the purpose of `<form>`?

Collects user input.

---

### Difference between GET and POST?

GET sends data through the URL.

POST sends data securely in the request body.

---

### Why use labels?

Improves accessibility and user experience.

---

### Difference between checkbox and radio?

Checkbox → Multiple selections.

Radio → Single selection.

---

### What is a placeholder?

A hint shown inside an input field.

---

# Summary

HTML forms are used to collect user input. They consist of form controls such as text fields, checkboxes, radio buttons, dropdowns, and buttons.