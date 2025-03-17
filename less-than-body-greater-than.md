---
icon: html5
---

# \<body>

The `<body>` tag in HTML represents the main content of a webpage that is displayed in the browser. Everything visible on the page, such as text, images, videos, and interactive elements, should be placed inside the `<body>` tag.

#### **Basic Structure:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Webpage</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph inside the body.</p>
</body>
</html>
```

#### **Key Points:**

* The `<body>` tag is placed inside the `<html>` tag and follows the `<head>` section.
* It contains all visible content like headings, paragraphs, images, and interactive elements.
* It does **not** support attributes for styling directly but can be styled using CSS.

#### **Example with Inline CSS:**

```html
<body style="background-color: lightblue; text-align: center;">
    <h1>Hello, World!</h1>
    <p>This page has a light blue background.</p>
</body>
```

Add a background image to a document (with CSS):

```html
<html>
<head>
<style>
body {
  background-image: url(w3s.png);
}
</style>
</head>
<body>

<h1>Hello world!</h1>
<p><a href="https://www.w3schools.com">Visit W3Schools.com!</a></p>

</body>
```

Set the background color of a document (with CSS):

```html
<html>
<head>
<style>
body {
  background-color: #E6E6FA;
}
</style>
</head>
<body>

<h1>Hello world!</h1>
<p><a href="https://www.w3schools.com">Visit W3Schools.com!</a></p>

</body>
```

Set the color of unvisited links in a document (with CSS):

```html
<html>
<head>
<style>
a:link {
  color:#0000FF;
}
</style>
</head>
<body>

<p><a href="https://www.w3schools.com">W3Schools.com</a></p>
<p><a href="https://www.w3schools.com/html/">HTML Tutorial</a></p>

</body>
</html>
```

Set the color of visited links in a document (with CSS):

```html
<!DOCTYPE html>
<html>
<head>
<style>
a:visited {
  color: #FF0000;
}
</style>
</head>
<body>

<p><a href="https://www.w3schools.com">W3Schools.com</a></p>
<p><a href="https://www.w3schools.com/html/">HTML Tutorial</a></p>

</body>
</html>

```
