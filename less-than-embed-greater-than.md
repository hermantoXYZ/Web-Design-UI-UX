---
icon: html5
---

# \<embed>

The `<embed>` tag in HTML is used to embed external content like videos, audio, PDFs, or other media files into a webpage. It is a **self-closing** tag and supports various attributes for customization.

***

#### **Basic Syntax:**

```html
<embed src="file.pdf" type="application/pdf" width="600" height="400">
```

***

#### **Common Uses of `<embed>`**

1.  **Embedding a PDF File**

    ```html
    <embed src="document.pdf" type="application/pdf" width="800" height="600">
    ```
2.  **Embedding an Audio File**

    ```html
    <embed src="audio.mp3" type="audio/mpeg">
    ```
3.  **Embedding a Video**

    ```html
    <embed src="video.mp4" type="video/mp4" width="640" height="360">
    ```
4.  **Embedding Flash Content (Deprecated)**

    ```html
    <embed src="flash.swf" type="application/x-shockwave-flash">
    ```

    ⚠ **Flash is outdated and no longer supported in modern browsers!**

***

#### **Key Attributes of `<embed>`**

| Attribute | Description                                                         |
| --------- | ------------------------------------------------------------------- |
| `src`     | Specifies the URL of the embedded content.                          |
| `type`    | Defines the MIME type (e.g., `application/pdf`, `video/mp4`, etc.). |
| `width`   | Sets the width of the embedded content.                             |
| `height`  | Sets the height of the embedded content.                            |

***

#### **Alternative to `<embed>`**

Instead of `<embed>`, it's often better to use:

* `<iframe>` for PDFs & external web pages.
* `<audio>` and `<video>` for media files.

Example using `<iframe>` for a PDF:

```html
<iframe src="document.pdf" width="800" height="600"></iframe>
```

