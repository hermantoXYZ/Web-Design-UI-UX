---
icon: html5
---

# HTML Basic Examples

In this chapter we will show some basic HTML examples.

Don't worry if we use tags you have not learned about yet.

***

### HTML Documents

All HTML documents must start with a document type declaration: `<!DOCTYPE html>`.

The HTML document itself begins with `<html>` and ends with `</html>`.

The visible part of the HTML document is between `<body>` and `</body>`.

```
// Some code
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

### The \<!DOCTYPE> Declaration

The `<!DOCTYPE>` declaration represents the document type, and helps browsers to display web pages correctly.

It must only appear once, at the top of the page (before any HTML tags).

The `<!DOCTYPE>` declaration is not case sensitive.

The `<!DOCTYPE>` declaration for HTML5 is:

`<!DOCTYPE html>`

***

### HTML Headings

HTML headings are defined with the `<h1>` to `<h6>` tags.

`<h1>` defines the most important heading. `<h6>` defines the least important heading:&#x20;

#### Example

```
// Some code
<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
```

### HTML Paragraphs

HTML paragraphs are defined with the `<p>` tag:

```
#Example 
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```

### HTML Links

HTML links are defined with the `<a>` tag:

#### Example

`<a href="https://www.w3schools.com">This is a link</a>`[`Try it Yourself »`](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_basic_link)

The link's destination is specified in the `href` attribute.&#x20;

Attributes are used to provide additional information about HTML elements.

You will learn more about attributes in a later chapter.

***

### HTML Images

HTML images are defined with the `<img>` tag.

The source file (`src`), alternative text (`alt`), `width`, and `height` are provided as attributes:

`<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">`[`Try it Yourself »`](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_basic_img)\
