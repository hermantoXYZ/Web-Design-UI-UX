---
icon: html5
---

# \<figure>

The `<figure>` tag in HTML is used to group media elements like images, illustrations, diagrams, or videos along with a caption (`<figcaption>`). It helps improve **semantic structure** and **accessibility** of a webpage.

***

#### **Basic Syntax:**

```html
<figure>
    <img src="image.jpg" alt="Description of image">
    <figcaption>This is an image caption.</figcaption>
</figure>
```

***

#### **Common Uses of `<figure>`**

1.  **Image with Caption**

    ```html
    <figure>
        <img src="sunset.jpg" alt="A beautiful sunset">
        <figcaption>Sunset over the ocean.</figcaption>
    </figure>
    ```
2.  **Video with Caption**

    ```html
    <figure>
        <video width="320" height="240" controls>
            <source src="video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
        <figcaption>A short clip of the ocean waves.</figcaption>
    </figure>
    ```
3.  **Diagram with Caption**

    ```html
    <figure>
        <img src="diagram.png" alt="Technical diagram">
        <figcaption>Figure 1: System Architecture.</figcaption>
    </figure>
    ```

***

#### **Key Benefits of Using `<figure>`**

* **Semantic HTML** – Helps search engines and screen readers understand the relationship between the media and its caption.
* **Better Organization** – Keeps images and captions together in a structured way.
* **Improves Accessibility** – `<figcaption>` provides context to users who rely on assistive technologies.

***

#### **Styling `<figure>` with CSS**

```html
<style>
    figure {
        border: 1px solid #ddd;
        padding: 10px;
        max-width: 400px;
        text-align: center;
    }
    figcaption {
        font-style: italic;
        color: #555;
    }
</style>

<figure>
    <img src="landscape.jpg" alt="Beautiful landscape" width="100%">
    <figcaption>A breathtaking view of the mountains.</figcaption>
</figure>
```

***

#### **Difference Between `<figure>` and `<img>`**

| Element    | Purpose                                                    |
| ---------- | ---------------------------------------------------------- |
| `<img>`    | Displays an image without additional structure.            |
| `<figure>` | Groups an image with an optional caption (`<figcaption>`). |

Would you like to see more advanced styling for `<figure>`? 😊
