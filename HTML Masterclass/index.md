# 📘 HTML Revision Notes
---

# What is HTML?

**HTML (HyperText Markup Language)** is the standard markup language used to create the structure of web pages.

HTML is **not a programming language**. It is a **markup language** that tells the browser how to display content.

---

# HTML Boilerplate

Every HTML document starts with a basic structure called the **HTML Boilerplate**.

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

## Explanation

| Tag | Purpose |
|------|---------|
| `<!DOCTYPE html>` | Declares the document as HTML5 |
| `<html>` | Root element of the webpage |
| `lang="en"` | Specifies the document language |
| `<head>` | Contains metadata |
| `<meta charset="UTF-8">` | Supports almost every character |
| `<meta viewport>` | Makes webpage responsive |
| `<title>` | Title shown on browser tab |
| `<body>` | Contains all visible webpage content |

---

# Heading Tags

HTML provides six heading levels.

```html
<h1>Heading</h1>
<h2>Heading</h2>
...
<h6>Heading</h6>
```

## Notes

- `<h1>` is the largest heading.
- `<h6>` is the smallest heading.
- Only one `<h1>` should generally be used per page.
- Headings improve SEO and accessibility.

---

# Paragraph Tag

```html
<p>Hello World</p>
```

Used for writing paragraphs.

---

# Text Formatting Tags

## Bold

```html
<b>Text</b>
```

Makes text bold.

---

## Strong

```html
<strong>Text</strong>
```

Makes text bold and indicates that the content is important.

Difference:

- `<b>` → Visual only.
- `<strong>` → Visual + Semantic.

---

## Italic

```html
<i>Text</i>
```

Displays italic text.

---

## Emphasis

```html
<em>Text</em>
```

Displays italic text with semantic emphasis.

Difference:

- `<i>` → Only italic.
- `<em>` → Italic + Meaning.

---

## Underline

```html
<u>Text</u>
```

Underlines the text.

---

# Horizontal Rule

```html
<hr>
```

Creates a horizontal line to separate content.

---

# Line Break

```html
<br>
```

Moves the next content to a new line.

---

# Superscript

```html
2<sup>2</sup>
```

Output

```
2²
```

Used for powers and exponents.

Examples

- x²
- 10³

---

# Subscript

```html
H<sub>2</sub>O
```

Output

```
H₂O
```

Used for chemical formulas.

Examples

- H₂O
- CO₂

---

# Lists

HTML provides three types of lists.

---

## Ordered List

Displays numbered items.

```html
<ol>
    <li>Apple</li>
    <li>Mango</li>
</ol>
```

### Attributes

| Attribute | Purpose |
|-----------|---------|
| reversed | Reverse numbering |
| start | Starting number |
| type | Numbering style |

Possible values of `type`

- 1
- A
- a
- I
- i

---

## Unordered List

Displays bulleted items.

```html
<ul>
    <li>Apple</li>
    <li>Mango</li>
</ul>
```

Bullet styles

- disc
- circle
- square
- none

---

## Description List

Used for terms and their descriptions.

```html
<dl>

<dt>HTML</dt>

<dd>HyperText Markup Language</dd>

</dl>
```

### Tags

| Tag | Purpose |
|------|---------|
| `<dl>` | Description List |
| `<dt>` | Description Term |
| `<dd>` | Description Definition |

---

# Anchor Tag

Used to create hyperlinks.

```html
<a href="https://example.com">
Visit Website
</a>
```

## Important Attributes

| Attribute | Purpose |
|-----------|---------|
| href | Link destination |
| target="_blank" | Opens link in new tab |

---

# Details Tag

Creates expandable content.

```html
<details>

<summary>Click Here</summary>

<p>Hello</p>

</details>
```

### Tags

| Tag | Purpose |
|------|---------|
| `<details>` | Expandable section |
| `<summary>` | Clickable heading |

---

# Select Tag

Creates a dropdown menu.

```html
<select>

<option>India</option>

<option>USA</option>

</select>
```

### Tags

| Tag | Purpose |
|------|---------|
| `<select>` | Dropdown |
| `<option>` | Dropdown option |

---

# Image Tag

Displays an image.

```html
<img src="image.jpg" alt="Image">
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| src | Image location |
| alt | Alternative text |
| width | Image width |
| height | Image height |

---

# Video Tag

Embeds videos.

```html
<video controls>

</video>
```

## Common Attributes

| Attribute | Purpose |
|-----------|---------|
| controls | Show controls |
| autoplay | Play automatically |
| muted | Mute audio |
| loop | Repeat video |

---

# Audio Tag

Embeds audio.

```html
<audio controls>

</audio>
```

## Common Attributes

- controls
- autoplay
- muted
- loop

---

# Table

Used to display tabular data.

```html
<table>

<tr>
<th>Name</th>
<th>City</th>
</tr>

<tr>
<td>Deva</td>
<td>Kanpur</td>
</tr>

</table>
```

### Table Tags

| Tag | Purpose |
|------|---------|
| `<table>` | Creates table |
| `<tr>` | Table row |
| `<th>` | Header cell |
| `<td>` | Data cell |

> **Note:** `border`, `bgcolor`, and `bordercolor` are deprecated in HTML5. Use CSS for styling.

---

# Forms

Forms collect user input.

```html
<form>

</form>
```

---

# Input Tag

The `<input>` tag allows users to enter data.

### Common Input Types

| Type | Purpose |
|------|---------|
| text | Single-line text |
| password | Hidden password |
| email | Email input |
| date | Date picker |
| checkbox | Multiple selection |
| radio | Single selection |
| file | File upload |

Example

```html
<input type="text">
```

---

# Label Tag

Associates text with an input field.

```html
<label for="email">Email</label>
```

---

# Button Tag

Creates a clickable button.

```html
<button>Submit</button>
```

---

# Common Input Attributes

| Attribute | Purpose |
|-----------|---------|
| placeholder | Hint text |
| required | Mandatory field |
| value | Default value |
| name | Field name |
| id | Unique identifier |
| type | Specifies input type |

---

# Semantic vs Non-Semantic Tags

| Non-Semantic | Semantic |
|--------------|----------|
| `<b>` | `<strong>` |
| `<i>` | `<em>` |

Semantic tags improve:

- Accessibility
- SEO
- Screen reader support

---

# Best Practices

- Use only one `<h1>` per page.
- Always provide an `alt` attribute for images.
- Connect `<label>` with `<input>` using the `for` attribute.
- Use semantic tags whenever possible.
- Give every form input a `name` attribute.
- Avoid deprecated HTML attributes like `bgcolor`.
- Keep HTML properly indented.
- Close all tags properly.
- Do not nest `<p>` tags inside another `<p>` tag.

---

# Quick Revision

| Tag | Purpose |
|------|---------|
| `<h1>` - `<h6>` | Headings |
| `<p>` | Paragraph |
| `<b>` | Bold |
| `<strong>` | Important text |
| `<i>` | Italic |
| `<em>` | Emphasized text |
| `<u>` | Underline |
| `<hr>` | Horizontal line |
| `<br>` | Line break |
| `<sup>` | Superscript |
| `<sub>` | Subscript |
| `<ol>` | Ordered List |
| `<ul>` | Unordered List |
| `<dl>` | Description List |
| `<dt>` | Description Term |
| `<dd>` | Description Definition |
| `<a>` | Hyperlink |
| `<details>` | Expandable section |
| `<summary>` | Summary heading |
| `<select>` | Dropdown |
| `<option>` | Dropdown item |
| `<img>` | Image |
| `<video>` | Video |
| `<audio>` | Audio |
| `<table>` | Table |
| `<tr>` | Table Row |
| `<th>` | Header Cell |
| `<td>` | Data Cell |
| `<form>` | Form |
| `<input>` | User Input |
| `<label>` | Label |
| `<button>` | Button |

---

# Topics Covered ✅

- HTML Introduction
- HTML Boilerplate
- Headings
- Paragraphs
- Text Formatting
- Lists
- Links
- Details & Summary
- Dropdowns
- Images
- Audio
- Video
- Tables
- Forms
- Input Types
- Labels
- Buttons
- Semantic HTML Basics

---
**Happy Coding! 🚀**