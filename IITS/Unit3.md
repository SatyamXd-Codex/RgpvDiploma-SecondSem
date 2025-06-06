
## UNIT 3: HTML4, CSS, and Making a Basic Personal Webpage

This unit introduces the core languages used to create web content and style it, culminating in the practical application of building a simple personal webpage.

### I. HTML4 (HyperText Markup Language 4)

HTML is the standard markup language for creating web pages and web applications. It uses a system of "tags" to structure content, defining elements like headings, paragraphs, images, and links. HTML4 was a widely adopted standard before the advent of HTML5, which brought significant new features. Understanding HTML4 principles is a solid foundation for modern web development.

#### A. Basic Structure of an HTML4 Document

A typical HTML4 document follows a specific structure:

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
    <title>Page Title</title>
    </head>
<body>
    </body>
</html>
```

* **`<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">`**: The Document Type Declaration (DTD). This line tells the web browser which version of HTML (in this case, HTML 4.01 Transitional) the page is written in.
* **`<html>`...`</html>`**: The root element that encloses all other HTML elements.
* **`<head>`...`</head>`**: Contains metadata about the HTML document that is not displayed directly on the webpage.
    * **`<title>`...`</title>`**: Defines the title that appears in the browser's title bar or tab.
    * **`<meta>` tags**: Provide various metadata about the page (e.g., character set, description, keywords).
    * **`<link>` tags**: Used to link to external resources, most commonly CSS stylesheets.
    * **`<script>` tags**: Used to embed or link to JavaScript code.
* **`<body>`...`</body>`**: Contains all the visible content of the web page, including text, images, links, tables, forms, etc.

#### B. Common HTML4 Tags and Their Usage

Here's a list of essential HTML4 tags and their purposes:

* **Headings:**
    * `<h1>` to `<h6>`: Define headings of different levels. `<h1>` is the most important, `<h6>` the least.
        * Example: `<h1>My Personal Webpage</h1>`
* **Paragraphs:**
    * `<p>`: Defines a paragraph of text.
        * Example: `<p>This is a paragraph of text on my webpage.</p>`
* **Line Breaks:**
    * `<br>`: Inserts a single line break. It's an empty tag (no closing tag).
        * Example: `Line 1<br>Line 2`
* **Horizontal Rule:**
    * `<hr>`: Creates a horizontal line, often used as a thematic break. It's an empty tag.
        * Example: `<hr>`
* **Text Formatting (Inline Elements):**
    * `<strong>` or `<b>`: Renders text in bold. `<strong>` has semantic importance (strong emphasis).
    * `<em>` or `<i>`: Renders text in italics. `<em>` has semantic importance (emphasis).
    * `<u>`: Underlined text (though often avoided for links).
    * `<strike>` or `<del>`: Strikethrough text (indicates deleted text).
    * `<sub>`: Subscript text.
    * `<sup>`: Superscript text.
* **Lists:**
    * **Unordered List:** `<ul>` (unordered list) with `<li>` (list item)
        * Example:
            ```html
            <ul>
                <li>Item 1</li>
                <li>Item 2</li>
            </ul>
            ```
    * **Ordered List:** `<ol>` (ordered list) with `<li>` (list item)
        * Example:
            ```html
            <ol>
                <li>First item</li>
                <li>Second item</li>
            </ol>
            ```
* **Links (Hyperlinks):**
    * `<a>` (anchor) with the `href` attribute: Creates a hyperlink to another page or resource.
        * Example: `<a href="https://www.google.com">Visit Google</a>`
        * `target="_blank"` attribute: Opens the link in a new tab/window.
            * Example: `<a href="page2.html" target="_blank">Go to Page 2</a>`
* **Images:**
    * `<img>` with `src` (source) and `alt` (alternative text) attributes: Embeds an image. It's an empty tag.
        * Example: `<img src="my_image.jpg" alt="Description of my image">`
        * `width` and `height` attributes (optional, for sizing):
            * Example: `<img src="logo.png" alt="Company Logo" width="100" height="50">`
* **Tables:**
    * `<table>`: Defines a table.
    * `<tr>`: Defines a table row.
    * `<th>`: Defines a table header cell.
    * `<td>`: Defines a table data cell.
        * Example:
            ```html
            <table>
                <tr>
                    <th>Header 1</th>
                    <th>Header 2</th>
                </tr>
                <tr>
                    <td>Data 1</td>
                    <td>Data 2</td>
                </tr>
            </table>
            ```
* **Divisions and Spans:**
    * `<div>`: A generic block-level container element. Used for grouping and styling larger sections of content.
    * `<span>`: A generic inline-level container element. Used for grouping and styling smaller pieces of content within a block.
        * Example: `<div>This is a <span style="color: blue;">blue</span> word.</div>`
* **Comments:**
    * ``: Used to add notes within the HTML code that are ignored by the browser.

### II. CSS (Cascading Style Sheets)

CSS is a stylesheet language used for describing the presentation of a document written in HTML (or XML). It controls the layout, colors, fonts, and overall visual appearance of web pages.

#### A. Why CSS is Used

* **Separation of Concerns:** Separates content (HTML) from presentation (CSS), making HTML cleaner and easier to maintain.
* **Consistency:** Allows applying consistent styles across multiple pages by linking a single CSS file.
* **Efficiency:** Changes to style can be made in one place (the CSS file) and applied to all pages linked to it, saving time.
* **Flexibility:** Allows adapting the presentation to different devices (e.g., desktops, tablets, mobile phones) using responsive design techniques.

#### B. Ways to Include CSS in an HTML Document

1.  **Inline Styles:**
    * **Description:** CSS rules are applied directly to an individual HTML element using the `style` attribute.
    * **Syntax:** `<p style="color: blue; font-size: 16px;">This text is blue.</p>`
    * **Pros:** Quick for single-use styling.
    * **Cons:** Not reusable, mixes content and presentation, difficult to maintain for larger projects. *Generally discouraged for most styling.*

2.  **Internal (Embedded) Styles:**
    * **Description:** CSS rules are placed within a `<style>` tag inside the `<head>` section of the HTML document.
    * **Syntax:**
        ```html
        <head>
            <style type="text/css">
                p {
                    color: green;
                    font-family: Arial;
                }
            </style>
        </head>
        ```
    * **Pros:** Styles apply to all elements within that single HTML page.
    * **Cons:** Not reusable across multiple pages, still mixes CSS with HTML, can make HTML file large.

3.  **External Stylesheets (Most Recommended):**
    * **Description:** CSS rules are written in a separate `.css` file and linked to the HTML document using the `<link>` tag in the `<head>` section.
    * **Syntax (in HTML file):** `<link rel="stylesheet" type="text/css" href="styles.css">`
    * **Syntax (in `styles.css` file):**
        ```css
        body {
            background-color: lightblue;
        }

        h1 {
            color: navy;
            text-align: center;
        }
        ```
    * **Pros:** Highly reusable across multiple pages, clean separation of concerns, easy to maintain.
    * **Cons:** Requires an additional HTTP request to fetch the CSS file.

#### C. Basic CSS Syntax (Selectors, Properties, Values)

A CSS rule consists of a selector and a declaration block.

* **Selector:** Points to the HTML element(s) you want to style.
* **Declaration Block:** Contains one or more declarations, separated by semicolons.
* **Declaration:** Consists of a CSS property name and a value, separated by a colon.

```css
selector {
    property: value;
    property2: value2;
}
```

* **Example:**
    ```css
    h1 {               /* Selector: targets all <h1> elements */
        color: blue;   /* Declaration 1: property is 'color', value is 'blue' */
        font-size: 24px; /* Declaration 2: property is 'font-size', value is '24px' */
    }

    .my-class {        /* Selector: targets all elements with class="my-class" */
        background-color: yellow;
    }

    #my-id {           /* Selector: targets the element with id="my-id" */
        border: 1px solid black;
    }
    ```

#### D. Common CSS Properties

* **Color and Background:**
    * `color`: Sets the text color.
    * `background-color`: Sets the background color of an element.
    * `background-image`: Sets a background image.
* **Text and Fonts:**
    * `font-family`: Sets the font typeface (e.g., `Arial, sans-serif`).
    * `font-size`: Sets the size of the font (e.g., `16px`, `1.2em`).
    * `font-weight`: Sets the thickness of characters (e.g., `bold`, `normal`, `700`).
    * `text-align`: Sets the horizontal alignment of text (e.g., `left`, `right`, `center`, `justify`).
    * `text-decoration`: Adds decoration to text (e.g., `underline`, `none`).
    * `line-height`: Sets the height of a line of text.
* **Box Model (Layout):** Every HTML element is treated as a box.
    * `width`, `height`: Sets the dimensions of the content area.
    * `padding`: Creates space between the content and the border of an element.
    * `border`: Sets the style, width, and color of the element's border.
    * `margin`: Creates space outside the border of an element, pushing other elements away.
* **Display:**
    * `display`: Controls how an element is displayed (e.g., `block`, `inline`, `inline-block`, `none`).
* **Positioning:**
    * `position`: Controls the positioning method of an element (e.g., `static`, `relative`, `absolute`, `fixed`).
    * `top`, `right`, `bottom`, `left`: Used with `position` to specify element location.

### III. Making a Basic Personal Webpage

Now, let's put it all together to create a simple personal webpage.

#### A. Planning the Content

Before coding, sketch out what you want on your page. A basic personal webpage might include:

1.  **A Title:** Your Name or "My Personal Page".
2.  **A Heading:** "Welcome to My Page" or "About Me".
3.  **An Image:** A profile picture or relevant image.
4.  **Some Text:** A brief introduction, your hobbies, interests, or skills.
5.  **A List:** Of hobbies, education, or skills.
6.  **Contact Information:** Email, social media links (optional).
7.  **Navigation (optional for a single page):** Links to different sections if the page is long, or to other pages if you expand later.

#### B. Step-by-Step Creation

**Step 1: Create an HTML File**

Open a plain text editor (like Notepad on Windows, TextEdit on Mac, or a code editor like VS Code).

Save the file as `index.html` (this is the standard filename for a homepage).

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
    <title>My Personal Webpage</title>
    <link rel="stylesheet" type="text/css" href="style.css"> </head>
<body>

    <h1>Welcome to My Personal Webpage!</h1>
    <hr>

    <img src="your_profile_picture.jpg" alt="My Profile Picture" width="200">

    <h2>About Me</h2>
    <p>Hello! My name is [Your Name]. I am a student interested in [Your Interests]. I enjoy learning about new technologies and how they shape our world.</p>

    <h2>My Hobbies</h2>
    <ul>
        <li>Reading books</li>
        <li>Playing [Your Sport/Game]</li>
        <li>Learning new [Skills/Languages]</li>
        <li>[Another Hobby]</li>
    </ul>

    <h2>Education</h2>
    <p>Currently pursuing a [Your Degree] at [Your College Name].</p>

    <h2>Contact Me</h2>
    <p>Email: <a href="mailto:your.email@example.com">your.email@example.com</a></p>
    <p>Connect with me on: <a href="https://linkedin.com/in/yourprofile" target="_blank">LinkedIn</a> (replace with your actual link)</p>

    <hr>
    <p style="text-align: center; font-size: small;">&copy; 2025 [Your Name]. All rights reserved.</p>

</body>
</html>
```

* **Remember to:**
    * Replace `your_profile_picture.jpg` with the actual filename of an image you place in the same folder as `index.html`.
    * Replace `[Your Name]`, `[Your Interests]`, `[Your Sport/Game]`, `[Skills/Languages]`, `[Your Degree]`, `[Your College Name]`, `your.email@example.com`, and the LinkedIn link with your actual details.

**Step 2: Create a CSS File**

In the **same folder** as `index.html`, create a new plain text file and save it as `style.css`.

```css
/* Basic styles for the personal webpage */

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4; /* Light grey background */
    color: #333; /* Dark grey text */
    margin: 20px; /* Space around the content */
    line-height: 1.6;
}

h1 {
    color: #0056b3; /* Dark blue heading */
    text-align: center;
    border-bottom: 2px solid #0056b3; /* Underline effect */
    padding-bottom: 10px;
}

h2 {
    color: #007bff; /* Medium blue heading */
    margin-top: 30px;
}

img {
    display: block; /* Make image a block element */
    margin: 0 auto; /* Center the image */
    border: 3px solid #ddd; /* Light grey border */
    border-radius: 8px; /* Slightly rounded corners */
    box-shadow: 2px 2px 5px rgba(0,0,0,0.2); /* Subtle shadow */
}

p {
    margin-bottom: 10px;
}

ul {
    list-style-type: square; /* Square bullet points */
    margin-left: 20px;
}

a {
    color: #007bff; /* Link color */
    text-decoration: none; /* No underline by default */
}

a:hover {
    text-decoration: underline; /* Underline on hover */
}

hr {
    border: 0;
    height: 1px;
    background-color: #ccc;
    margin: 20px 0;
}
```

**Step 3: Add an Image (Optional but Recommended)**

Find a small image (e.g., a profile picture) and save it in the **same folder** as `index.html` and `style.css`. Make sure its filename matches what you put in the `<img>` tag (`your_profile_picture.jpg` in the example).

**Step 4: View Your Webpage**

Navigate to the folder where you saved `index.html`. Double-click on `index.html`. It should open in your default web browser, displaying your very first personal webpage with basic styling!
