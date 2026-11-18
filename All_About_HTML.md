# All About HTML — Complete Beginner to Advanced Guide

**A free, practical HTML course for beginners**

Author: K M Imran Hossen  
Level: Beginner → Intermediate → Advanced  
Language: English (with simple explanations and practical examples)  
Technology: HTML5

---

## How to use this guide

1. Install [Visual Studio Code](https://code.visualstudio.com/) and a modern browser such as Chrome or Firefox.
2. Create a folder named `All_About_HTML`.
3. Inside it, create a file named `index.html`.
4. Copy the examples from this guide into your file and save it.
5. Open the HTML file in your browser. Edit the code and refresh the browser to see your changes.
6. Practise the exercises at the end of each chapter.
7. Upload your notes and projects to your own GitHub repository.

> HTML describes the structure and meaning of web content. CSS controls presentation, while JavaScript adds behaviour and interactivity.

## Table of contents

1. What HTML is
2. Your first HTML page
3. Elements, tags and attributes
4. Headings, paragraphs and text
5. Links and navigation
6. Images and figures
7. Lists
8. Tables
9. Forms and input controls
10. Semantic HTML
11. Audio, video and embedded content
12. Metadata and the document head
13. Global attributes
14. Special characters and entities
15. HTML accessibility
16. HTML validation and good practices
17. SEO basics
18. Useful HTML elements reference
19. Complete practice projects
20. Exercises and mini quiz
21. Suggested learning path and resources

---

# 1. What is HTML?

HTML means **HyperText Markup Language**. It is the standard markup language used to structure content on web pages.

HTML is not a programming language. It uses elements (written with tags) to describe content such as headings, paragraphs, images, links, tables and forms.

### A simple example

```html
<h1>Welcome</h1>
<p>This is my first web page.</p>
```

- `<h1>` marks the main heading.
- `<p>` marks a paragraph.
- The browser interprets the markup and displays the content.

### HTML, CSS and JavaScript

| Technology | Main job |
|---|---|
| HTML | Structure and meaning |
| CSS | Layout, colours, typography and visual design |
| JavaScript | Interaction and dynamic behaviour |

### What you need

- A code editor: Visual Studio Code is a popular free option.
- A web browser: Chrome, Firefox, Edge or Safari.
- A folder for your practice files.

**Practice:** Create a folder called `html-practice`. Inside it, create `index.html`.

---

# 2. Your first HTML page

An HTML document has a standard basic structure.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Web Page</title>
</head>
<body>
    <h1>Hello, world!</h1>
    <p>I am learning HTML.</p>
</body>
</html>
```

### Understand each part

- `<!DOCTYPE html>` tells the browser to use modern HTML.
- `<html lang="en">` is the root element and declares the document language.
- `<head>` contains document information that is not ordinary page content.
- `<meta charset="UTF-8">` sets the character encoding.
- The viewport meta tag helps the page scale on mobile devices.
- `<title>` sets the browser tab title.
- `<body>` contains the page content shown in the browser.

### How to run it

1. Save the file as `index.html`.
2. Find the file in File Explorer.
3. Double-click it to open it in your browser.
4. Change the heading, save, and refresh the browser.

**Exercise:** Make a page with your name as the heading and three sentences about yourself.

---

# 3. Elements, tags and attributes

An HTML **element** commonly consists of an opening tag, content and a closing tag.

```html
<p>This is a paragraph.</p>
```

- Opening tag: `<p>`
- Content: `This is a paragraph.`
- Closing tag: `</p>`
- Complete element: the whole line

Some elements are void elements and do not have closing tags or child content. Examples include `<img>`, `<br>`, `<hr>` and `<input>`.

### Nesting elements

Elements can be placed inside other elements. They must be nested correctly.

```html
<p>This is <strong>important</strong> text.</p>
```

Correct nesting closes the inner element before the outer element.

### Attributes

Attributes provide extra information about an element. They are written in the opening tag.

```html
<a href="https://example.com" target="_blank" rel="noopener">
    Visit Example
</a>
```

- `href` specifies the link destination.
- `target="_blank"` opens the link in a new tab.
- `rel="noopener"` is a security best practice for new-tab links.

### Attribute rules

- Put attributes in the opening tag.
- Most attribute values should be quoted.
- Attribute names are generally written in lowercase.
- An element can have multiple attributes.

**Exercise:** Create a link to a website you use regularly. Give it meaningful link text.

---

# 4. Headings, paragraphs and text

### Headings

HTML provides six heading levels: `<h1>` through `<h6>`.

```html
<h1>Main page heading</h1>
<h2>Major section</h2>
<h3>Subsection</h3>
<h4>Smaller section</h4>
<h5>Minor heading</h5>
<h6>Lowest-level heading</h6>
```

Use headings to organise the page hierarchy, not simply to make text large. Usually, a page has one clear main heading.

### Paragraphs and line breaks

```html
<p>This is the first paragraph.</p>
<p>This is the second paragraph.</p>

<p>First line<br>Second line</p>
<hr>
<p>Content after a thematic break.</p>
```

- `<p>` creates a paragraph.
- `<br>` creates a line break within text when the break is meaningful.
- `<hr>` represents a thematic break between sections.

Do not use repeated `<br>` elements to create page spacing; use CSS for layout.

### Text meaning and emphasis

```html
<p><strong>Important:</strong> Save your work regularly.</p>
<p><em>Please read the instructions carefully.</em></p>
<p><b>Bold presentation</b> and <i>alternate voice</i>.</p>
<p><mark>Highlighted text</mark></p>
<p><small>Small print or side comments.</small></p>
<p><del>Old price</del> <ins>New price</ins></p>
<p>Water is H<sub>2</sub>O.</p>
<p>2<sup>3</sup> = 8.</p>
```

Use `<strong>` for importance and `<em>` for stress emphasis. `<b>` and `<i>` do not carry the same semantic emphasis.

### Quotations and code

```html
<blockquote cite="https://example.com">
    A longer quotation placed in its own block.
</blockquote>

<p>She said, <q>Keep practising.</q></p>

<p>Use the <code>console.log()</code> function in JavaScript.</p>

<pre><code>
function greet() {
    return "Hello!";
}
</code></pre>
```

- `<blockquote>` is for an extended quotation.
- `<q>` is for a short inline quotation.
- `<code>` marks computer code.
- `<pre>` preserves whitespace and line breaks.

**Exercise:** Create an article with one `<h1>`, two `<h2>` headings, three paragraphs, one important sentence and one quotation.

---

# 5. Links and navigation

The anchor element `<a>` creates a hyperlink.

### External link

```html
<a href="https://developer.mozilla.org/">Learn HTML on MDN</a>
```

### Open in a new tab

```html
<a href="https://example.com" target="_blank" rel="noopener">
    Open Example
</a>
```

### Link to another page in your project

```html
<a href="about.html">About</a>
```

### Link to a section on the same page

```html
<a href="#contact">Go to contact section</a>

<section id="contact">
    <h2>Contact</h2>
    <p>Contact information goes here.</p>
</section>
```

### Email and telephone links

```html
<a href="mailto:hello@example.com">Send an email</a>
<a href="tel:+8801000000000">Call us</a>
```

### Relative and absolute URLs

- Absolute URL: a complete address such as `https://example.com/about`.
- Relative URL: a path relative to the current document, such as `about.html` or `images/photo.jpg`.

**Exercise:** Create a navigation list linking to Home, About, Projects and Contact sections.

---

# 6. Images and figures

Use `<img>` to place an image on a page.

```html
<img src="images/profile.jpg" alt="Portrait of the website author" width="300">
```

Important attributes:

- `src`: image path or URL.
- `alt`: text alternative describing the image's purpose.
- `width` and `height`: image dimensions; setting both can help the browser reserve space.

### Figure and caption

```html
<figure>
    <img src="images/mountain.jpg"
         alt="A mountain rising above a green valley"
         width="600">
    <figcaption>A mountain landscape.</figcaption>
</figure>
```

### Image best practices

- Use descriptive alternative text for informative images.
- Use `alt=""` for purely decorative images.
- Keep image files in an organised folder.
- Use suitable image formats and compress large files.
- Do not use an image of text when real text can be used.

**Exercise:** Add a profile image to your personal page and write suitable alternative text.

---

# 7. Lists

### Unordered list

Use `<ul>` when the order does not matter.

```html
<h2>My skills</h2>
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

### Ordered list

Use `<ol>` when sequence matters.

```html
<h2>How to create a web page</h2>
<ol>
    <li>Create a project folder.</li>
    <li>Create an index.html file.</li>
    <li>Write HTML code.</li>
    <li>Open it in a browser.</li>
</ol>
```

### Description list

```html
<dl>
    <dt>HTML</dt>
    <dd>Structures web content.</dd>

    <dt>CSS</dt>
    <dd>Controls the presentation of web content.</dd>
</dl>
```

Lists can be nested by placing a list inside an `<li>`.

**Exercise:** Create a shopping list and a numbered recipe.

---

# 8. Tables

Use tables for genuinely tabular data, not for general page layout.

```html
<table>
    <caption>Weekly study schedule</caption>
    <thead>
        <tr>
            <th scope="col">Day</th>
            <th scope="col">Subject</th>
            <th scope="col">Hours</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope="row">Monday</th>
            <td>HTML</td>
            <td>2</td>
        </tr>
        <tr>
            <th scope="row">Tuesday</th>
            <td>CSS</td>
            <td>2</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <th scope="row" colspan="2">Total hours</th>
            <td>4</td>
        </tr>
    </tfoot>
</table>
```

### Important table elements

- `<table>`: the table.
- `<caption>`: a title or description.
- `<thead>`: header rows.
- `<tbody>`: main data rows.
- `<tfoot>`: summary rows.
- `<tr>`: a row.
- `<th>`: a header cell.
- `<td>`: a data cell.

### Spanning cells

- `colspan="2"` makes a cell span two columns.
- `rowspan="2"` makes a cell span two rows.

Use header cells and appropriate `scope` values to help users understand the relationships in a table.

**Exercise:** Build a marks table with columns for subject, total marks and obtained marks.

---

# 9. Forms and input controls

Forms collect information from users.

### Basic form

```html
<form action="/submit" method="post">
    <label for="full-name">Full name</label>
    <input type="text" id="full-name" name="fullName" required>

    <label for="email">Email address</label>
    <input type="email" id="email" name="email" required>

    <button type="submit">Submit</button>
</form>
```

A form needs a server-side endpoint or suitable JavaScript to process submitted data. HTML alone does not store or email form submissions.

### Common input types

```html
<form>
    <label for="name">Name</label>
    <input type="text" id="name" name="name">

    <label for="password">Password</label>
    <input type="password" id="password" name="password">

    <label for="age">Age</label>
    <input type="number" id="age" name="age" min="1" max="120">

    <label for="birthday">Date of birth</label>
    <input type="date" id="birthday" name="birthday">

    <label for="colour">Favourite colour</label>
    <input type="color" id="colour" name="colour">

    <label for="website">Website</label>
    <input type="url" id="website" name="website">

    <label for="search">Search</label>
    <input type="search" id="search" name="search">

    <label for="resume">Upload a file</label>
    <input type="file" id="resume" name="resume">

    <button type="submit">Send</button>
</form>
```

### Radio buttons

Radio buttons allow one choice from a group. Use the same `name` for the group.

```html
<fieldset>
    <legend>Select your level</legend>

    <input type="radio" id="beginner" name="level" value="beginner">
    <label for="beginner">Beginner</label>

    <input type="radio" id="advanced" name="level" value="advanced">
    <label for="advanced">Advanced</label>
</fieldset>
```

### Checkboxes

Checkboxes allow multiple selections.

```html
<fieldset>
    <legend>Choose your interests</legend>

    <input type="checkbox" id="html" name="interest" value="html">
    <label for="html">HTML</label>

    <input type="checkbox" id="css" name="interest" value="css">
    <label for="css">CSS</label>
</fieldset>
```

### Select menu and textarea

```html
<label for="country">Country</label>
<select id="country" name="country">
    <option value="">Choose a country</option>
    <option value="bd">Bangladesh</option>
    <option value="in">India</option>
</select>

<label for="message">Message</label>
<textarea id="message" name="message" rows="5"></textarea>
```

### Useful form attributes

- `name`: key used when form data is submitted.
- `value`: submitted value.
- `required`: field must be completed.
- `placeholder`: short hint, not a replacement for a label.
- `min` and `max`: numeric or date limits where supported.
- `minlength` and `maxlength`: text length limits.
- `checked` and `selected`: initial selection states.
- `disabled`: makes a control unavailable.
- `readonly`: prevents editing while keeping the value available for submission.

### GET and POST

- `GET` generally sends form data as URL query parameters and is suitable for retrieval/search forms.
- `POST` sends data in the request body and is commonly used for actions that submit or change data.
- Neither method replaces server-side validation and security.

**Exercise:** Build a student registration form with name, email, date of birth, gender choice, interests, department selection and a submit button.

---

# 10. Semantic HTML

Semantic elements describe the purpose of different parts of a page.

```html
<body>
    <header>
        <h1>My Learning Website</h1>
        <nav aria-label="Main navigation">
            <a href="#home">Home</a>
            <a href="#lessons">Lessons</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <main id="home">
        <section id="lessons">
            <h2>HTML Lessons</h2>
            <article>
                <h3>Introduction to HTML</h3>
                <p>Learn the structure of a web page.</p>
            </article>
        </section>

        <aside>
            <h2>Quick tip</h2>
            <p>Practise a little every day.</p>
        </aside>
    </main>

    <footer id="contact">
        <p>Copyright 2026 My Learning Website</p>
    </footer>
</body>
```

Common semantic elements:

- `<header>`: introductory content for a page or section.
- `<nav>`: a major navigation area.
- `<main>`: the main content of the page.
- `<section>`: a thematic section, usually with a heading.
- `<article>`: self-contained content.
- `<aside>`: related or supplementary content.
- `<footer>`: footer information for a page or section.
- `<address>`: contact information for the relevant person or organisation.

Prefer semantic elements when they accurately describe the content. Do not choose an element merely because of its default appearance.

---

# 11. Audio, video and embedded content

### Audio

```html
<audio controls>
    <source src="media/audio.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```

### Video

```html
<video controls width="640" poster="images/video-cover.jpg">
    <source src="media/lesson.mp4" type="video/mp4">
    Your browser does not support the video element.
</video>
```

Useful media attributes include `controls`, `autoplay`, `muted`, `loop`, `poster`, `width` and `height`. Autoplay can be disruptive; avoid it unless there is a clear reason. Browsers commonly restrict autoplay with sound.

### Captions

For video captions, use a WebVTT file:

```html
<video controls width="640">
    <source src="media/lesson.mp4" type="video/mp4">
    <track src="captions/lesson-en.vtt"
           kind="captions"
           srclang="en"
           label="English"
           default>
</video>
```

### Iframe

```html
<iframe
    src="https://www.example.com/"
    title="Example website"
    width="600"
    height="400"
    loading="lazy">
</iframe>
```

Only embed content from sources you trust. Some websites block embedding.

**Exercise:** Add an audio player and a video player to a media page.

---

# 12. Metadata and the document head

The `<head>` element contains information about the document.

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Beginner-friendly HTML lessons and examples.">
    <title>HTML Learning Guide</title>
    <link rel="icon" href="images/favicon.png">
    <link rel="stylesheet" href="css/style.css">
</head>
```

- `<title>`: document title shown in browser tabs and often used in search results.
- Description metadata: a short summary of the page.
- Favicon: small site icon.
- Stylesheet link: connects an external CSS file.

Metadata should accurately describe the page. Search engines may choose a different snippet from the page content.

---

# 13. Global attributes

Global attributes can be used on many HTML elements.

```html
<p id="intro" class="highlight" title="Introduction paragraph">
    Welcome to the course.
</p>

<p lang="en">This paragraph is in English.</p>

<div data-course-level="beginner">
    Beginner lesson
</div>

<p hidden>This content is hidden.</p>
```

Common global attributes:

- `id`: unique identifier within a document.
- `class`: one or more class names, often used by CSS and JavaScript.
- `style`: inline CSS; generally prefer external stylesheets for maintainability.
- `title`: advisory information, not a replacement for accessible labels.
- `lang`: language of the element's content.
- `dir`: text direction, such as `ltr` or `rtl`.
- `hidden`: indicates that content should not be displayed.
- `data-*`: custom data attributes for scripts and applications.
- `tabindex`: controls focusability and keyboard navigation; use carefully.

---

# 14. Special characters and entities

Some characters have special meaning in HTML and should be written using character references when they are intended as text.

| Character | Entity |
|---|---|
| `<` | `&lt;` |
| `>` | `&gt;` |
| `&` | `&amp;` |
| `"` | `&quot;` |
| Non-breaking space | `&nbsp;` |
| © | `&copy;` |
| ® | `&reg;` |

Example:

```html
<p>Use &lt;h1&gt; for a main heading.</p>
<p>Copyright &copy; 2026.</p>
```

Save documents as UTF-8 so that text in different languages can be represented correctly.

---

# 15. HTML accessibility

Accessible HTML helps people with different abilities use websites.

### Important practices

1. Use semantic elements for structure.
2. Use a logical heading hierarchy.
3. Give every form control a visible, associated label.
4. Add useful alternative text to informative images.
5. Use descriptive link text such as “Read the HTML guide” rather than “Click here”.
6. Make sure the page can be used with a keyboard.
7. Use buttons for actions and links for navigation.
8. Provide captions or transcripts for relevant audio and video.
9. Set the document language with the `lang` attribute.
10. Do not communicate meaning using colour alone.

### Label example

```html
<label for="email-address">Email address</label>
<input type="email" id="email-address" name="email" required>
```

### Button versus link

```html
<a href="about.html">Read about us</a>
<button type="button">Open menu</button>
```

A link navigates to a resource. A button performs an action.

---

# 16. HTML validation and good practices

### Good coding habits

- Use lowercase element and attribute names.
- Indent nested elements consistently.
- Quote attribute values.
- Give images meaningful `alt` text.
- Use unique IDs in a document.
- Close non-void elements correctly.
- Use semantic HTML.
- Keep CSS and JavaScript in separate files for larger projects.
- Use meaningful file and folder names.
- Test pages at different screen sizes and with a keyboard.

### Validate your HTML

Use the [Nu HTML Checker](https://validator.w3.org/nu/) to find markup errors and warnings. Validation does not guarantee that a page is accessible, secure or well-designed, but it is a useful quality check.

### Common beginner mistakes

- Forgetting `<!DOCTYPE html>`.
- Putting visible page content inside `<head>` instead of `<body>`.
- Using duplicate `id` values.
- Forgetting an image's `alt` attribute.
- Using headings only to change text size.
- Using tables for page layout.
- Using placeholder text instead of form labels.
- Expecting an HTML form to save data without a server or script.

---

# 17. SEO basics for HTML authors

Search engine optimisation (SEO) is broader than HTML, but clear markup helps search engines and people understand a page.

```html
<head>
    <title>Beginner HTML Course | My Learning Site</title>
    <meta name="description"
          content="Learn HTML with simple explanations, examples and projects.">
</head>
<body>
    <main>
        <h1>Beginner HTML Course</h1>
        <p>Learn to structure web pages with practical HTML examples.</p>
    </main>
</body>
```

Good starting practices:

- Give each page a clear, descriptive title.
- Write a useful meta description.
- Use meaningful headings.
- Create descriptive links.
- Use helpful image alternative text.
- Publish useful, original content.
- Make pages mobile-friendly and fast.

Avoid keyword stuffing and misleading titles.

---

# 18. Useful HTML elements reference

| Element | Purpose |
|---|---|
| `<html>` | Root of an HTML document |
| `<head>` | Document metadata and resource links |
| `<title>` | Browser/document title |
| `<body>` | Visible document content |
| `<h1>`–`<h6>` | Headings |
| `<p>` | Paragraph |
| `<a>` | Hyperlink |
| `<img>` | Image |
| `<ul>` / `<ol>` | Unordered / ordered list |
| `<li>` | List item |
| `<table>` | Tabular data |
| `<tr>` | Table row |
| `<th>` / `<td>` | Table header / data cell |
| `<form>` | Form |
| `<label>` | Form control label |
| `<input>` | Input control |
| `<textarea>` | Multiline text input |
| `<button>` | Button |
| `<select>` / `<option>` | Selection control / option |
| `<header>` | Introductory area |
| `<nav>` | Navigation |
| `<main>` | Main content |
| `<section>` | Thematic section |
| `<article>` | Self-contained composition |
| `<aside>` | Related content |
| `<footer>` | Footer |
| `<figure>` / `<figcaption>` | Figure and caption |
| `<audio>` / `<video>` | Media players |
| `<iframe>` | Embedded browsing context |
| `<div>` | Generic block container |
| `<span>` | Generic inline container |
| `<br>` | Line break |
| `<hr>` | Thematic break |

This is a learning reference, not a complete list of every HTML element or attribute. Consult MDN for detailed specifications and browser support.

---

# 19. Complete practice projects

Create a separate folder for each project. Each project should have its own `index.html` file.

## Project 1: Personal profile page

Requirements:

- Page title and main heading.
- Profile image with suitable alternative text.
- About-me paragraph.
- Skills list.
- Links to projects and contact information.
- Semantic header, main and footer.

Starter code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Profile</title>
</head>
<body>
    <header>
        <h1>Your Name</h1>
        <p>Student | Web Development Learner</p>
    </header>

    <main>
        <section>
            <h2>About Me</h2>
            <p>Write a short introduction about yourself.</p>
        </section>

        <section>
            <h2>My Skills</h2>
            <ul>
                <li>HTML</li>
                <li>Problem solving</li>
            </ul>
        </section>

        <section>
            <h2>Contact</h2>
            <a href="mailto:you@example.com">Email me</a>
        </section>
    </main>

    <footer>
        <p>Copyright 2026 Your Name</p>
    </footer>
</body>
</html>
```

## Project 2: Student registration form

Requirements:

- Full name and email.
- Date of birth.
- Department dropdown.
- Radio button group.
- Multiple interest checkboxes.
- Message textarea.
- Submit button.
- Correct labels and required fields.

## Project 3: Course timetable

Requirements:

- A descriptive table caption.
- Header row with column headings.
- At least five schedule rows.
- Correct use of `<th>` and `<td>`.
- A total or summary row.

## Project 4: Small multi-page website

Create these files:

```text
my-website/
├── index.html
├── about.html
├── courses.html
├── contact.html
└── images/
```

Requirements:

- Navigation between all pages.
- A clear heading on each page.
- Relevant content and images.
- A contact form with labels.
- Consistent semantic structure.

---

# 20. Exercises and mini quiz

Try these without looking at the examples first.

### Practical exercises

1. Create a valid HTML document from scratch.
2. Add six heading levels and three paragraphs.
3. Create an external link and an internal page link.
4. Add an image with useful alternative text.
5. Create ordered, unordered and description lists.
6. Build a table showing five students and their marks.
7. Create a form with text, email, password, radio and checkbox controls.
8. Structure a page using header, nav, main, section, article and footer.
9. Add an audio or video player.
10. Build a four-page personal website.

### Mini quiz

**1. What does HTML stand for?**

A. HyperText Markup Language  
B. HighText Machine Language  
C. Hyper Transfer Main Language  
D. Home Tool Markup Language

**2. Which element creates the largest standard heading level?**

A. `<head>`  
B. `<h6>`  
C. `<h1>`  
D. `<heading>`

**3. Which attribute provides alternative text for an image?**

A. `src`  
B. `alt`  
C. `title`  
D. `href`

**4. Which element creates a hyperlink?**

A. `<link>`  
B. `<href>`  
C. `<a>`  
D. `<url>`

**5. Which element is used for a form label?**

A. `<label>`  
B. `<caption>`  
C. `<legend>`  
D. `<name>`

**6. Which method is commonly used to submit data that changes server-side information?**

A. `GET`  
B. `POST`  
C. `LINK`  
D. `OPEN`

**7. Which element represents the main content of a page?**

A. `<aside>`  
B. `<footer>`  
C. `<main>`  
D. `<nav>`

**8. Which element is a void element?**

A. `<p>`  
B. `<section>`  
C. `<img>`  
D. `<article>`

**9. Which attribute should be unique within a document?**

A. `class`  
B. `id`  
C. `title`  
D. `style`

**10. Is HTML a programming language?**

A. Yes  
B. No; it is a markup language

### Answer key

1. A  
2. C  
3. B  
4. C  
5. A  
6. B  
7. C  
8. C  
9. B  
10. B

---

# 21. Suggested learning path and resources

## Recommended order

1. Learn the document structure and basic elements.
2. Practise text, links, images and lists.
3. Learn tables and forms.
4. Understand semantic HTML and accessibility.
5. Build the four projects in this guide.
6. Validate your pages and upload them to GitHub.
7. Move on to CSS, then JavaScript.

## Free learning resources

- [MDN — HTML](https://developer.mozilla.org/en-US/docs/Web/HTML): detailed reference and guides.
- [W3Schools — HTML Tutorial](https://www.w3schools.com/html/): beginner-friendly explanations and examples.
- [freeCodeCamp](https://www.freecodecamp.org/learn/): interactive lessons and practice.
- [Nu HTML Checker](https://validator.w3.org/nu/): check HTML markup.
- [Visual Studio Code](https://code.visualstudio.com/): free code editor.

## Completion checklist

- [ ] I can create a valid HTML document.
- [ ] I understand tags, elements and attributes.
- [ ] I can add headings, paragraphs, links and images.
- [ ] I can create lists and data tables.
- [ ] I can build accessible forms.
- [ ] I understand semantic HTML.
- [ ] I can add audio, video and embedded content.
- [ ] I can use metadata and global attributes.
- [ ] I can validate and improve my HTML.
- [ ] I have completed at least three practice projects.

---

## License and contribution

This learning guide is provided for educational use. You may study it, practise with the examples and adapt your own notes. If you share or modify this guide, retain the author attribution and check the licences of any third-party resources you add.

**Keep practising. Build projects. Share what you learn.**
