---
icon: html5
---

# \<a>

The `<a>` tag in HTML is used to define hyperlinks, allowing users to navigate to other web pages, sections within the same page, or external resources. It stands for **"anchor"**.

#### Basic Syntax:

```html
<a href="https://example.com">Visit Example</a>
```

This creates a clickable link that directs users to `https://example.com`.

***

#### Attributes of `<a>` Tag:

1.  **`href`** – Specifies the URL of the link destination.

    ```html
    <a href="https://google.com">Google</a>
    ```
2.  **`target`** – Defines how the link will open:

    * `_self` (default): Opens in the same tab.
    * `_blank`: Opens in a new tab.
    * `_parent`: Opens in the parent frame.
    * `_top`: Opens in the full body of the window.

    ```html
    <a href="https://google.com" target="_blank">Open in new tab</a>
    ```
3.  **`title`** – Adds a tooltip when hovering over the link.

    ```html
    <a href="https://example.com" title="Go to Example">Hover over me</a>
    ```
4.  **`download`** – Specifies that the link should download a file instead of navigating to it.

    ```html
    <a href="file.pdf" download>Download PDF</a>
    ```
5.  **`rel`** – Defines the relationship between the current document and the linked URL.

    * `nofollow`: Tells search engines not to follow the link.
    * `noopener noreferrer`: Improves security for `_blank` links.

    ```html
    <a href="https://example.com" target="_blank" rel="noopener noreferrer">Safe Link</a>
    ```
6.  **`id` and `class`** – Useful for styling and JavaScript interaction.

    ```html
    <a href="#section1" id="myLink" class="nav-link">Jump to Section</a>
    ```
7. **`name`** – Used for internal navigation (deprecated, use `id` instead).

***

#### Internal Page Navigation (Anchor Links)

Can link to a section within the same page using an `id`:

```html
<a href="#about">Go to About Section</a>

<section id="about">
    <h2>About Us</h2>
</section>
```

***

#### Button-Like `<a>` Tag (With CSS)

To style an `<a>` tag like a button:

```html
<a href="https://example.com" class="btn">Click Me</a>

<style>
    .btn {
        display: inline-block;
        padding: 10px 20px;
        background: blue;
        color: white;
        text-decoration: none;
        border-radius: 5px;
    }
</style>
```
