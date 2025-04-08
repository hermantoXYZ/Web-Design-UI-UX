---
icon: html5
---

# \<!DOCTYPE>

`<!DOCTYPE>` is a declaration used in HTML and XHTML that specifies the document type and version being used. It helps the web browser understand how to display the content correctly by defining the standard rules for that document. For example, in an HTML5 document, the declaration is `<!DOCTYPE html>`.



```
<!DOCTYPE html>
<html>
<head>
<title>Title of the document</title>
</head>

<body>
The content of the document......
</body>

</html>
```

### Definition and Usage

All HTML documents must start with a `<!DOCTYPE>` declaration.

The declaration is not an HTML tag. It is an "information" to the browser about what document type to expect.

In HTML 5, the declaration is simple:

```html
<!DOCTYPE html>
```

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

### Older HTML Documents

In older documents (HTML 4 or XHTML), the declaration is more complicated because the declaration must refer to a DTD (Document Type Definition).

**HTML 4.01:**

{% code overflow="wrap" %}
```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```
{% endcode %}

**XHTML 1.1:**

{% code overflow="wrap" %}
```html

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">tn
```
{% endcode %}

