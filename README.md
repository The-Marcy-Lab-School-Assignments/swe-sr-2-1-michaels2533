# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Do some research on semantic and non-semantic elements and share your findings. Your response should include:

- Examples of semantic and non-semantic tags
- The differences between semantic and non-semantic tags
- The benefits of using semantic tags (when possible)

### Response 1

_Semantic tags_ are used to define the meaning of the content contained inside them. On the other hand, _non-semantic tags_ are content placeholders and don't indicate the type of content they contain.

Some examples of semantic tags are **header**, **footer** and **article** they describe the role of the content contained within them. An example of non-semantic tags would be a **div** or **span** they hold information without specifying the meaning.

The benefits of using semantic tags include greater accessibility, search engine optimization, easier to read and a better user experience.

## Prompt 2

Do some research on accessibility. What are some ways to make your website more accessible? Explain why it is important for developers to create websites that meet accessibility standards.

### Response 2

There are many ways to ensure your website is accessible to a wide range of users. Some strategies you could use are:

- Use of Semantic HTML to create a cohesive structure for your web content. In turn, assistive software can better interpret your website.
- Provide text alternatives for audio, video and text content this includes alternate text descriptions for images and transcriptions of videos/audio content.
- Keyboard-Friendly Design that ensures the website can be navigated via keyboard for users that can't use a mouse.

The adhering to accessibility standards is important because you want to provide equal access to a larger user base. Additionally, ensuring you're complying with the accessibility laws in your jurisdiction. Finally, more accessible websites are generally more user-friendly thus improving user engagement and satisfaction.

## Prompt 3

It is possible to add "inline" CSS styles to our html elements using the `style` attribute like so:

```html
<p style="color: red;">hello world</p>
```

While this is possible, it is a best practice to instead write styles in a separate CSS file. Provide at least one argument for why it _might_ be considered useful to write inline styles, and then provide a more compelling argument for writing styles in a separate CSS file.

### Response 3

A reason that a developer might even consider using inline styling is styling a element with a single attribute. In this case, creating a separate CSS file would simply be unnecessary. Although, If they ever wanted to add more styling in the future it would be difficult. Therefore, keeping in mind the idea of separation of concerns encourages scalability, maintainability and reusability.

## Prompt 4

Imagine you are teaching a brand new programmer a brief lesson about the `class` and `id` attributes in HTML as well as how to use them to style elements using CSS. Your lesson should have the following components:

- An explanation of the concept of "classes" and "ids" with an analogy.
- An example of the usage using an HTML code block and a CSS code block.
- An explanation of the syntax using the terms: **attribute**, **selector**

### Response 4

The _class_ and _id_ attributes are ways to organize and style our HTML elements. A _class_ would be like a team name and multiple people (HTML elements) can belong to the same team. On the other hand, you can think of a _id_ like a driver license because it's unique to one individual(HTML element).

Here's a code example using class and id attributes.

HTML File:

```
<!DOCTYPE html>
<html lang="en">
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <h1 id="main-heading">Welcome to My Website</h1>
  <p class="text">This is the first paragraph.</p>
  <p class="text">This is the second paragraph.</p>
</body>
</html>
```

In the HTML file, the class and id attributes are put inside the opening tags of the HTML element. As you can see each attribute is assigned a custom name. This name can be used to reference the class or id in a separate CSS file.

CSS File:

```
/* Selector for the 'id' attribute */
#main-heading {
  color: blue;
  font-size: 32px;
}

/* Selector for the 'class' attribute */
.text {
  color: green;
  font-size: 18px;
}
```

In the CSS file, a selector is used to assign various properties to the selected attribute. A important thing to note is the id selectors begin with the pound character(#) while the class selector begins with a period. Furthermore, this is used to distinguish between the two types of HTML attributes.

## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

### Response 5

When developing a website use HTML and CSS for static content and styling. As this will ensure maintainability, good performance and accessability. However reserve the Javascript and DOM manipulation for the dynamic/interactive content. For instance, updating user-specific information, handling events and fetching data from an API. In conclusion, the separation of concerns improves readability,performance and reduces complexity.
