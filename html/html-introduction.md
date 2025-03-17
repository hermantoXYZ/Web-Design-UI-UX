---
description: HTML is the standard markup language for creating Web pages.
icon: html5
---

# HTML Introduction

### What is HTML?

* HTML stands for Hyper Text Markup Language
* HTML is the standard markup language for creating Web pages
* HTML describes the structure of a Web page
* HTML consists of a series of elements
* HTML elements tell the browser how to display the content
* HTML elements label pieces of content such as "this is a heading", "this is a paragraph", "this is a link", etc.

### A Simple HTML Document

```html
// Some code
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

#### Example Explained

* The `<!DOCTYPE html>` declaration defines that this document is an HTML5 document
* The `<html>` element is the root element of an HTML page
* The `<head>` element contains meta information about the HTML page
* The `<title>` element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
* The `<body>` element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
* The `<h1>` element defines a large heading
* The `<p>` element defines a paragraph

\
What is an HTML Element?

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

| Start tag | Element content     | End tag |
| --------- | ------------------- | ------- |
| \<h1>     | My First Heading    | \</h1>  |
| \<p>      | My first paragraph. | \</p>   |
| \<br>     | _none_              | _none_  |

{% hint style="danger" %}
**Note:** Some HTML elements have no content (like the \<br> element). These elements are called empty elements. Empty elements do not have an end tag!
{% endhint %}

The purpose of a web browser (Chrome, Edge, Firefox, Safari) is to read HTML documents and display them correctly.

A browser does not display the HTML tags, but uses them to determine how to display the document:

![View in Browser](https://www.w3schools.com/html/img_chrome.png)

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

<details>

<summary>What does HTML stand for?</summary>

```
// Some code
Hot Typing Markup Language
Home Typing Modern Language
Hyper Text Markup Language
Home Testing Mixed Language
```

</details>

