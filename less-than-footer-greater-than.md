# \<footer>

The `<footer>` tag in HTML is used to define the footer section of a webpage or a section of content. It typically contains information like copyright notices, links, contact details, or related navigation.

***

#### **Basic Syntax:**

```html
<footer>
    <p>&copy; 2025 My Website. All rights reserved.</p>
</footer>
```

***

#### **Common Uses of `<footer>`**

1.  **Website Footer with Navigation**

    ```html
    <footer>
        <p>&copy; 2025 MyWebsite</p>
        <nav>
            <a href="about.html">About</a> |
            <a href="contact.html">Contact</a> |
            <a href="privacy.html">Privacy Policy</a>
        </nav>
    </footer>
    ```
2.  **Footer Inside an Article**

    ```html
    <article>
        <h2>Blog Post Title</h2>
        <p>Content of the blog post...</p>
        <footer>Written by John Doe | Published on March 17, 2025</footer>
    </article>
    ```
3.  **Footer with Social Media Links**

    ```html
    <footer>
        <p>Follow us on:</p>
        <a href="https://twitter.com">Twitter</a> |
        <a href="https://facebook.com">Facebook</a> |
        <a href="https://instagram.com">Instagram</a>
    </footer>
    ```

***

#### **Styling `<footer>` with CSS**

```html
<style>
    footer {
        background-color: #222;
        color: white;
        text-align: center;
        padding: 15px;
        font-size: 14px;
    }

    footer a {
        color: #ffcc00;
        text-decoration: none;
        margin: 0 10px;
    }

    footer a:hover {
        text-decoration: underline;
    }
</style>

<footer>
    <p>&copy; 2025 MyWebsite | <a href="privacy.html">Privacy Policy</a></p>
</footer>
```

***

#### **Key Points About `<footer>`**

✅ Used for **page-wide** or **section-wide** footers.\
✅ Typically contains **copyright info, navigation links, and contact details**.\
✅ Can be placed inside `<article>` or `<section>` for content-specific footers.

Would you like help designing a modern responsive footer? 😊
