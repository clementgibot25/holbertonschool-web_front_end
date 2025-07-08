# HTML5 Advanced Concepts

## Table of Contents
1. [HTML Guidelines](#html-guidelines)
2. [HTML5 Page Skeleton](#html5-page-skeleton)
3. [Semantic HTML Tags](#semantic-html-tags)
4. [Div vs Span](#div-vs-span)
5. [Semantic Elements Explained](#semantic-elements-explained)
6. [Headings Hierarchy](#headings-hierarchy)
7. [HTML Lists](#html-lists)
8. [Image Formats Comparison](#image-formats-comparison)
9. [HTML Tables](#html-tables)
10. [Embedding Video](#embedding-video)
11. [Embedding Audio](#embedding-audio)
12. [External Content](#external-content)
13. [HTML Page Structure](#html-page-structure)

## HTML Guidelines

### General Guidelines
- Always declare `<!DOCTYPE html>` at the beginning
- Use lowercase for element and attribute names
- Always quote attribute values
- Always include alt attributes for images
- Use semantic elements where appropriate
- Keep nesting to a minimum
- Use proper indentation (2 or 4 spaces)
- Close all HTML elements properly

### Accessibility Guidelines
- Use proper heading structure (h1-h6)
- Add alt text for images
- Use ARIA attributes when necessary
- Ensure sufficient color contrast
- Make interactive elements keyboard accessible

## HTML5 Page Skeleton

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Page description">
    <title>Page Title</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Page content goes here -->
    <script src="script.js"></script>
</body>
</html>
```

## Semantic HTML Tags

Semantic HTML tags clearly describe their meaning to both the browser and the developer. Examples include:

- `<header>`: Represents introductory content
- `<nav>`: Navigation links
- `<main>`: Main content
- `<article>`: Self-contained composition
- `<section>`: Thematic grouping of content
- `<aside>`: Sidebar content
- `<footer>`: Footer content
- `<figure>` and `<figcaption>`: For images with captions
- `<time>`: For dates and times

## Div vs Span

### `<div>` (Block-level)
- Used for layout and grouping block-level elements
- Creates a block-level box
- Used for larger sections of content
- Example:
  ```html
  <div class="container">
      <h1>Title</h1>
      <p>Content</p>
  </div>
  ```

### `<span>` (Inline)
- Used for styling or scripting inline portions of text
- Creates an inline box
- Used for smaller, inline elements
- Example:
  ```html
  <p>This is <span class="highlight">important</span> text.</p>
  ```

## Semantic Elements Explained

| Element   | Purpose | Example |
|-----------|---------|---------|
| `<header>` | Introductory content | Page header with logo and navigation |
| `<main>`  | Main content of the document | Main article content |
| `<footer>` | Footer content | Copyright info, contact details |
| `<article>` | Self-contained composition | Blog post, news article |
| `<nav>`   | Navigation links | Main menu, table of contents |
| `<section>` | Thematic grouping | Chapters, tabbed content |
| `<aside>`  | Side content | Sidebar, pull quotes |

## Headings Hierarchy

Headings should follow a logical hierarchy:

```html
<h1>Main Title (only one per page)</h1>
  <h2>Main Section</h2>
    <h3>Subsection</h3>
    <h3>Another Subsection</h3>
      <h4>Sub-subsection</h4>
  <h2>Another Main Section</h2>
```

### Why It's Important:
- Improves accessibility for screen readers
- Helps search engines understand content structure
- Creates a clear document outline
- Makes content more scannable for users

## HTML Lists

### Unordered List
```html
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>
```

### Ordered List
```html
<ol>
    <li>First step</li>
    <li>Second step</li>
    <li>Third step</li>
</ol>
```

### Definition List
```html
<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>
    <dt>CSS</dt>
    <dd>Cascading Style Sheets</dd>
</dl>
```

## Image Formats Comparison

| Format | Best For | Advantages | Disadvantages |
|--------|----------|------------|---------------|
| **SVG** | Logos, icons, simple graphics | Scalable, small file size, editable with code | Not suitable for complex images |
| **GIF** | Simple animations, small animations | Supports animation, transparency | Limited to 256 colors, larger file size |
| **PNG** | Images with transparency, logos, screenshots | Lossless compression, supports transparency | Larger file size than JPG |
| **JPG/JPEG** | Photographs, complex images | Good compression, small file size | Lossy compression, no transparency |
| **WebP** | Modern alternative to JPG/PNG | Better compression, supports transparency | Not supported in older browsers |

## HTML Tables

```html
<table>
    <caption>Monthly Savings</caption>
    <thead>
        <tr>
            <th>Month</th>
            <th>Savings</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>January</td>
            <td>$100</td>
        </tr>
        <tr>
            <td>February</td>
            <td>$150</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td>Total</td>
            <td>$250</td>
        </tr>
    </tfoot>
</table>
```

## Embedding Video

### HTML5 Video
```html
<video width="640" height="360" controls>
    <source src="video.mp4" type="video/mp4">
    <source src="video.webm" type="video/webm">
    Your browser does not support the video tag.
</video>
```

### YouTube Embed
```html
<iframe width="560" height="315" 
        src="https://www.youtube.com/embed/VIDEO_ID" 
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
</iframe>
```

## Embedding Audio

```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    <source src="audio.ogg" type="audio/ogg">
    Your browser does not support the audio element.
</audio>
```

## External Content

### Embedding a Map
```html
<iframe src="https://www.google.com/maps/embed?pb=!1m18..." 
        width="600" 
        height="450" 
        style="border:0;" 
        allowfullscreen="" 
        loading="lazy">
</iframe>
```

### Embedding a Tweet
```html
<blockquote class="twitter-tweet">
    <p>Example tweet text</p>
    &mdash; Twitter User (@user) 
    <a href="https://twitter.com/user/status/12345">Month Day, Year</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js"></script>
```

## HTML Page Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Page description">
    <title>Document Title</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <!-- Navigation content -->
        </nav>
    </header>

    <main>
        <article>
            <header>
                <h1>Article Title</h1>
                <p>Published on <time datetime="2023-01-01">January 1, 2023</time></p>
            </header>
            
            <section>
                <h2>Introduction</h2>
                <p>Article content...</p>
            </section>
            
            <section>
                <h2>Main Content</h2>
                <p>More content...</p>
            </section>
        </article>

        <aside>
            <h3>Related Links</h3>
            <ul>
                <li><a href="#">Related Article 1</a></li>
                <li><a href="#">Related Article 2</a></li>
            </ul>
        </aside>
    </main>

    <footer>
        <p>&copy; 2023 Your Name. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
```

## Best Practices

1. **Validation**: Always validate your HTML using the [W3C Markup Validation Service](https://validator.w3.org/)
2. **Performance**: Optimize images and media files
3. **Accessibility**: Use proper ARIA attributes and semantic elements
4. **SEO**: Use proper heading structure and meta tags
5. **Responsive Design**: Use viewport meta tag and responsive units
6. **Progressive Enhancement**: Build core functionality first, then enhance
7. **Performance**: Load scripts asynchronously when possible
8. **Security**: Use HTTPS for all resources
9. **Maintainability**: Comment your code and follow consistent formatting
10. **Testing**: Test in multiple browsers and devices
