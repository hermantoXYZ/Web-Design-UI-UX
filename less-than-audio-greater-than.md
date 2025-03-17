---
icon: html5
---

# \<audio>

The `<audio>` tag in HTML is used to embed sound content, such as music or audio recordings, into a webpage. It supports multiple audio formats and provides playback controls.

#### Basic Syntax:

```html
<audio controls>
    <source src="audio-file.mp3" type="audio/mpeg">
    <source src="audio-file.ogg" type="audio/ogg">
    Your browser does not support the audio element.
</audio>
```

#### Attributes:

* **`controls`** – Displays play, pause, and volume controls.
* **`autoplay`** – Automatically plays the audio when the page loads.
* **`loop`** – Repeats the audio continuously.
* **`muted`** – Starts the audio in a muted state.
* **`preload`** – Specifies how the browser should load the audio file (`auto`, `metadata`, `none`).

#### Example with Autoplay and Loop:

```html
<audio controls autoplay loop>
    <source src="background-music.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```

