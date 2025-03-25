---
hidden: true
icon: html5
---

# \<abbr>

The `<abbr>` tag in HTML is used to define an **abbreviation** or **acronym**, providing additional information when the user hovers over the text. It enhances accessibility and usability by showing the full meaning of a shortened term.

***

#### **Basic Syntax:**

```html
<abbr title="HyperText Markup Language">HTML</abbr>
```

✅ When you hover over **"HTML"**, a tooltip will display **"HyperText Markup Language"**.

***

#### **Attributes of `<abbr>`:**

1.  **`title`** – Required attribute that specifies the full meaning of the abbreviation.

    ```html
    <abbr title="World Health Organization">WHO</abbr>
    ```
2.  **Global Attributes** – Supports attributes like `id`, `class`, `style`, etc.

    ```html
    <abbr id="abbr-example" class="highlight" title="JavaScript">JS</abbr>
    ```

***

#### **Example with Styling:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Abbr Example</title>
    <style>
        abbr {
            text-decoration: underline dotted;
            cursor: help;
        }
    </style>
</head>
<body>
    <p>The <abbr title="Cascading Style Sheets">CSS</abbr> language is used for styling web pages.</p>
</body>
</html>
```

✅ This adds a **dotted underline** to the abbreviation, making it clear that more information is available.

***

#### **Use Cases:**

* **Technical Terms**: `<abbr title="Application Programming Interface">API</abbr>`
* **Company/Organization Names**: `<abbr title="National Aeronautics and Space Administration">NASA</abbr>`
* **Medical Terms**: `<abbr title="Coronavirus Disease 2019">COVID-19</abbr>`
* **Educational Content**: `<abbr title="Doctor of Philosophy">Ph.D.</abbr>`
