
# Class 1 Reading Notes

### Review Questions

#### Getting Started

1. Compose a short poem describing how HTTP sends data between computers.

Web requests take flight,
Data flows in packets light,
HTTP makes it right.

2. Describe how HTML, CSS, and JS files are “parsed” in the browser.

HTML file, it readsfrom top to bottom.
CSS reads from top to bottom
JS can change the content and appearance, the browser will often pause HTML and CSS parsing

3. How can you find images to add to a Website?

Searching for hosted images or hosting a image online.

4. How do you create a String vs a Number in JavaScript?

Numbers don't have quotes around them.
To signify that the value is a string, enclose it in single or double quote marks.

5. What is a Variable and why are they important in JavaScript?

A variable is a container for a value, like a number we might use in a sum, or a string that we might use as part of a sentence. example

### HTML
<button id="button_A">Press me</button>
<h3 id="heading_A"></h3>

### JS
const buttonA = document.querySelector("#button_A");
const headingA = document.querySelector("#heading_A");

buttonA.onclick = () => {
  const name = prompt("What is your name?");
  alert(`Hello ${name}, nice to see you!`);
  headingA.textContent = `Welcome ${name}`;
};

#### Introduction to HTML

1. What is an HTML attribute?

HTML (HyperText Markup Language) is a markup language that tells web browsers how to structure the web pages you visit. It can be as complicated or as simple as the web developer wants it to be. HTML consists of a series of elements, which you use to enclose, wrap, or mark up different parts of content to make it appear or act in a certain way. The enclosing tags can make content into a hyperlink to connect to another page, italicize words, and so on. For example, consider the following line of text:

My cat is very grumpy
If we wanted the text to stand by itself, we could specify that it is a paragraph by enclosing it in a paragraph (<p>) element:

HTML
Copy to Clipboard

<p>My cat is very grumpy</p>

In HTML, an attribute provides additional information about an element and helps define its properties or behavior. Attributes are always specified in the opening tag of an element and come in name/value pairs like this: `name="value"`.

Here's a basic breakdown of how attributes work:

1. **Name**: This is the name of the attribute. It defines the property you want to set. The attribute name is case-insensitive, but it's a common practice to write them in lowercase.

2. **Value**: This is the value you want to set for the named property. The value is always enclosed in quotation marks, either single (`' '`) or double (`" "`). However, there are some boolean attributes (like `checked`, `disabled`, `readonly`, etc.) where the mere presence of the attribute implies a `true` value.

**Examples**:

- **`href` attribute for the `<a>` element**: This attribute specifies the URL the link points to.
  ```html
  <a href="https://www.example.com">Visit Example.com</a>
  ```

- **`src` attribute for the `<img>` element**: This attribute specifies the path to the image file.
  ```html
  <img src="path/to/image.jpg" alt="Description of Image">
  ```

- **`alt` attribute for the `<img>` element**: This provides a text alternative for the image, which can be read by screen readers or displayed if the image fails to load.
  ```html
  <img src="path/to/image.jpg" alt="Description of Image">
  ```

- **`class` and `id` attributes**: These are used for styling and scripting. The `class` attribute can be applied to multiple elements, while the `id` should be unique within a page.
  ```html
  <div class="container">...</div>
  <p id="uniqueParagraph">...</p>
  ```

Attributes enhance the functionality and presentation of HTML elements, allowing developers to configure them in various ways and make them interactive. They play a crucial role in making web content structured, styled, and interactive.

2. Describe the Anatomy of an HTMl element.

The anatomy of our element is:

The opening tag: This consists of the name of the element (in this example, p for paragraph), wrapped in opening and closing angle brackets. This opening tag marks where the element begins or starts to take effect. In this example, it precedes the start of the paragraph text.
The content: This is the content of the element. In this example, it is the paragraph text.
The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This marks where the element ends. Failing to include a closing tag is a common beginner error that can produce peculiar results.
The element is the opening tag, followed by content, followed by the closing tag.

https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started/grumpy-cat-small.png

3. What is the Difference between *article* and *section* element tags?

Both article and section are semantic HTML elements introduced in HTML5 to help structure content in a meaningful way. They provide better clarity about the content they enclose, not only for developers but also for browsers and assistive technologies. Let's dive into the differences:

Article Element:

Purpose: Represents a self-contained composition in a document, page, application, or site. This means that the content inside an <article> is independent and can make sense on its own, outside of its context. If you were to syndicate or republish it elsewhere, it would still retain its meaning.
Examples: Blog posts, news stories, forum posts, or comments.

4. What Elements does a “typical” website include?


main> is for content unique to this page. Use main> only once per page, and put it directly inside body>. Ideally this shouldn't be nested within other elements.

article> encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post).

section> is similar to article>, but it is more for grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme. It's considered best practice to begin each section with a heading; also note that you can break article>s up into different section>s, or section>s up into different article>s, depending on the context.

aside> contains content that is not directly related to the main content but can provide additional information indirectly related to it (glossary entries, author biography, related links, etc.).

header> represents a group of introductory content. If it is a child of body> it defines the global header of a webpage, but if it's a child of an article> or section> it defines a specific header for that section (try not to confuse this with titles and headings).

nav> contains the main navigation functionality for the page. Secondary links, etc., would not go in the navigation.

footer> represents a group of end content for a page.

5. How does metadata influence Search Engine Optimization?

Metadata plays a crucial role in Search Engine Optimization (SEO) because it provides search engines with information about the content of a web page, allowing them to understand, categorize, and rank the page appropriately.

6. How is the meta> HTML tag used when specifying metadata?

The meta> tag in HTML is used to provide metadata about the content of a webpage. 


####  How to start to design a Website.

1. What is the first step to designing a Website?
 List all the goals you want to reach.

2. What is the most important question to answer when designing a Website?
How can a website help me reach my goals?

#### Semantics.

1. Why should you use an <h1> element over a <span> element to display a top level heading?

Most browser's user agent stylesheet will style an h1 with a large font size to make it look like a heading

Span: will render it to look like a top level heading, but it has no semantic value, so it will not get any extra benefits.


2. What are the benefits of using semantic tags in our HTML?

In summary, using semantic tags in HTML not only makes the content more understandable for machines (like search engines and screen readers) but also for human developers. This practice leads to more accessible, search-friendly, and maintainable web content.

#### What is JavaScript?

1. Describe 2 things that require JavaScript in the Browser?

Dynamic Content Interaction & Manipulation

Web-Based Animations & Effects

2. How can you add JavaScript to an HTML document?

Internal JavaScript

External JavaScript

Inline JavaScript handlers