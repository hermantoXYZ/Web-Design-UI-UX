---
icon: html5
---

# \<div>

The `<div>` tag in HTML is a **container element** used to group and structure content. It does not have any semantic meaning but is commonly used for styling, layout, and JavaScript interactions.

***

#### **Basic Syntax:**

```html
<div>
    <p>This is a paragraph inside a div.</p>
</div>
```

***

#### **Common Uses of `<div>`:**

1.  **Grouping Elements for Styling**

    ```html
    <div style="background-color: lightgray; padding: 10px;">
        <h2>Title</h2>
        <p>Some content inside a div.</p>
    </div>
    ```
2.  **Creating Page Layouts (with CSS)**

    ```html
    <div class="container">
        <div class="header">Header Section</div>
        <div class="content">Main Content</div>
        <div class="footer">Footer Section</div>
    </div>
    ```
3.  **Using `<div>` with JavaScript**

    ```html
    <div id="myDiv">Click me</div>

    <script>
        document.getElementById("myDiv").addEventListener("click", function() {
            alert("Div clicked!");
        });
    </script>
    ```

***

#### **CSS Styling Example:**

```html
<style>
    .box {
        width: 200px;
        height: 100px;
        background-color: skyblue;
        text-align: center;
        padding: 20px;
        margin: 10px;
        border-radius: 10px;
    }
</style>

<div class="box">This is a styled div</div>
```

***

#### **Key Points:**

1. **No semantic meaning** – only used for grouping content.
2. **Works well with CSS & JavaScript** for layouts and dynamic interactions.
3. **Avoid excessive `<div>` nesting** (use semantic elements like `<section>`, `<article>`, `<aside>` where applicable).
