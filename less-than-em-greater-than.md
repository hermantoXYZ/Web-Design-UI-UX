---
icon: html5
---

# \<em>

The `<em>` tag in HTML is used to emphasize text, typically rendering it in _italic_ style. It also conveys semantic importance, which helps with accessibility and search engine optimization (SEO).

***

#### **Basic Syntax:**

```html
<p>This is <em>important</em> text.</p>
```

***

#### **Key Points About `<em>`:**

* It **adds emphasis** to the text for screen readers and SEO.
* It **renders text in italics** by default.
* If nested (`<em><em>text</em></em>`), it adds **stronger emphasis**.

***

#### **Example Usage:**

1.  **Basic Text Emphasis**

    ```html
    <p>Please <em>do not forget</em> to submit your assignment.</p>
    ```
2.  **Using `<em>` in a Sentence**

    ```html
    <p>She said, <em>"I really love programming!"</em></p>
    ```
3.  **Styled `<em>` with CSS**

    ```html
    <style>
        em {
            color: red;
            font-style: italic;
            font-weight: bold;
        }
    </style>

    <p>This is <em>important</em> text.</p>
    ```

***

#### **Difference Between `<em>` and `<i>`:**

| Tag    | Purpose                          | Default Style |
| ------ | -------------------------------- | ------------- |
| `<em>` | Emphasizes text (semantic)       | _Italic_      |
| `<i>`  | Stylistic italics (non-semantic) | _Italic_      |

👉 Use `<em>` when the emphasis **matters for meaning** (e.g., instructions, important phrases). Use `<i>` for **decorative purposes** (e.g., book titles, foreign words).

***
