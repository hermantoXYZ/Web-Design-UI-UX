---
icon: html5
---

# \<button>

The `<button>` tag in HTML is used to create a clickable button on a webpage. It can be used to trigger actions such as submitting forms, executing JavaScript functions, or navigating to other pages.

***

#### **Basic Syntax:**

```html
<button>Click Me</button>
```

***

#### **Types of Buttons:**

1.  **Default Button** (No type specified, behaves like a submit button inside a form)

    ```html
    <button>Default Button</button>
    ```
2.  **Submit Button** (Submits a form)

    ```html
    <button type="submit">Submit</button>
    ```
3.  **Reset Button** (Resets form fields)

    ```html
    <button type="reset">Reset</button>
    ```
4.  **Button for JavaScript Action**

    ```html
    <button type="button" onclick="alert('Hello!')">Click Me</button>
    ```

***

#### **Button with an Icon (Using FontAwesome)**

```html
<button>
    <i class="fas fa-download"></i> Download
</button>
```

(Requires FontAwesome library)

***

#### **Styled Button (Using CSS)**

```html
<style>
    button {
        background-color: #008CBA;
        color: white;
        padding: 10px 20px;
        border: none;
        cursor: pointer;
        font-size: 16px;
    }
    button:hover {
        background-color: #005f73;
    }
</style>

<button>Styled Button</button>
```

***

#### **Disabled Button**

```html
<button disabled>Disabled</button>
```

***

#### **Button Inside a Form**

```html
<form action="/submit-form" method="POST">
    <button type="submit">Submit Form</button>
</form>
```

