# HTML Mastery Notes

## 1. Introduction to HTML

### What is HTML?

- **HTML (HyperText Markup Language)** is the standard language for creating web pages.
- It allows users to structure content such as text, images, and links for display in web browsers.

### Why was HTML created?

- HTML was created by **Tim Berners-Lee** in 1991 to enable the sharing of documents and information over the internet.
- It was designed to be simple, enabling scientists and researchers to share data without the need for proprietary software.
- The primary goal of HTML was to create a universal, platform-independent way to structure and link content.

### How does HTML work?

1. **Document Structure**:
   - HTML documents are plain text files that use tags to define elements.
   - Tags provide instructions to the browser about how to display content.
2. **Elements and Tags**:

   - HTML uses **elements** enclosed in **tags** (e.g., `<p>` for a paragraph).
   - Tags are written in pairs with an opening `<tag>` and a closing `</tag>`.

3. **Browser Rendering**:
   - Browsers read HTML files and interpret the tags to render the content visually.
   - HTML works in conjunction with **CSS** (for styling) and **JavaScript** (for interactivity).

### Basic Structure of an HTML Document

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    <h1>Welcome to HTML</h1>
    <p>This is a basic HTML page.</p>
  </body>
</html>
```

- `<!DOCTYPE html>`: Declares the document type as HTML5.
- `<html>`: The root element of an HTML document.
- `<head>`: Contains metadata (e.g., title, meta tags).
- `<body>`: Contains the visible content of the webpage.

---

## 2. Tags and Attributes

### What are Tags?

- Tags are the building blocks of HTML.
- They define elements on a webpage, such as headings, paragraphs, or images.
- Tags are written in angle brackets: `<tag>`.
- Most tags come in pairs:
  - Opening tag: `<p>`
  - Closing tag: `</p>`

Example:

```html
<p>This is a paragraph.</p>
```

### What are Attributes?

- Attributes provide additional information about an HTML element.
- They are written inside the opening tag.
- Syntax: `<tag attribute="value">`.
- Example:
  ```html
  <a href="https://example.com" target="_blank">Visit Example</a>
  ```
  - `href`: Specifies the link's URL.
  - `target`: Defines where to open the link.

### Key Points about Attributes

1. **Attributes always appear inside the opening tag.**
2. **They have a name and a value**, separated by an equals sign.
3. **Values are always enclosed in quotes** (single or double).

Example with multiple attributes:

```html
<img src="image.jpg" alt="A beautiful image" width="600" height="400" />
```

- `src`: Path to the image file.
- `alt`: Alternative text for accessibility.
- `width` and `height`: Dimensions of the image.

---

## 3. Common HTML Elements

### Headings

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Smaller Subheading</h3>
```

- Headings range from `<h1>` (largest) to `<h6>` (smallest).

### Paragraphs

```html
<p>This is a paragraph.</p>
```

### Links

```html
<a href="https://example.com">Visit Example</a>
```

- `href`: Specifies the URL of the link.

### Images

```html
<img src="image.jpg" alt="Description of image" />
```

- `src`: Path to the image file.
- `alt`: Text to display if the image cannot load.

### Lists

#### Ordered List

```html
<ol>
  <li>First item</li>
  <li>Second item</li>
</ol>
```

#### Unordered List

```html
<ul>
  <li>First item</li>
  <li>Second item</li>
</ul>
```

---

## 4. Semantic HTML

- Semantic tags clearly define the purpose of the content.

### Common Semantic Tags

```html
<header>
  <h1>Page Header</h1>
</header>

<nav>
  <a href="#">Home</a>
  <a href="#">About</a>
</nav>

<main>
  <article>
    <h2>Article Title</h2>
    <p>Content of the article.</p>
  </article>
</main>

<footer>
  <p>&copy; 2024 My Website</p>
</footer>
```

### Importance of Semantic HTML

- **Accessibility**: Semantic HTML improves accessibility for screen readers and other assistive technologies.
- **SEO**: Search engines use semantic tags to better understand the content of a webpage, which can improve search rankings.
- **Maintainability**: Semantic HTML makes the code easier to read and maintain.
- **Collaboration**: Clear structure and meaning make it easier for multiple developers to work on the same project.

---

## 5. Forms

- Used to collect user input.

### Example:

```html
<form action="/submit" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required />

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" />

  <button type="submit">Submit</button>
</form>
```

- `action`: URL to send the form data.
- `method`: HTTP method (`get` or `post`).
- `required`: Makes a field mandatory.

---

## 6. Media

### Video

```html
<video controls>
  <source src="video.mp4" type="video/mp4" />
  Your browser does not support the video tag.
</video>
```

### Audio

```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg" />
  Your browser does not support the audio tag.
</audio>
```

---

## 7. Tables

```html
<table>
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
    </tr>
  </tbody>
</table>
```

- `<thead>`, `<tbody>`, `<tfoot>`: Define table sections.
- `<tr>`: Table row.
- `<th>`: Header cell.
- `<td>`: Data cell.

---

## 8. Advanced Topics

### HTML Entities

- Special characters:

```html
&lt; ( < ) &gt; ( > ) &amp; ( & )
```

### Inline vs Block Elements

- **Inline Elements**:
  - Do not start on a new line.
  - Examples: `<span>`, `<a>`, `<img>`.
- **Block Elements**:
  - Always start on a new line.
  - Examples: `<div>`, `<p>`, `<h1>`.

### Identifying Inline and Block Elements

- Use the **Inspect Tool** in Chrome:
  1. Right-click on the element and select **Inspect**.
  2. Select the inspect tools present in the right top corner like in the following image:
     ![alt text](image.png)
  3. Hover of the the element to see if it covers the entire line/block. If it does that then it is block elements otherwise it is a inline element.

### Inline Frames (iFrame)

```html
<iframe src="https://example.com" width="600" height="400"></iframe>
```

---

## 9. Best Practices

1. **Use semantic HTML** for better accessibility and SEO.
2. **Keep code clean and indented** for readability.
3. **Use comments** to explain complex sections:
   ```html
   <!-- This is a comment -->
   ```
4. Validate HTML using [W3C Validator](https://validator.w3.org/).
5. Use external CSS and JavaScript instead of inline styles/scripts.

---

## 10. Resources for Further Learning

- [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [W3Schools HTML Tutorial](https://www.w3schools.com/html/)
- [HTML Validator](https://validator.w3.org/)
