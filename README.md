# Clear and Consistent Sass Variable Naming with EPM Structure

**EPM** - Element Property Modifier

This project provides a naming convention for Sass variables built on the **Element-Property-Modifier (EPM)** structure. This method promotes clear, consistent, and scalable variable naming, leading to:

- **Improved readability and maintainability:** Code is easier to understand and navigate for both you and your team.
- **Reduced errors and duplication:** Consistent naming minimizes mistakes and redundant variables.
- **Flexibility and scalability:** The structure easily accommodates complex UI components and future growth.

This project includes examples, usage guidelines, and potential benefits to help you implement EPM effectively in your Sass projects.

## Examples

### Element: `.button`

HTML
```html
<button class='button'></button>
```

Sass variables
```scss
$button__color: #fff;
$button__color--hover: #000;
$button__font-family--sans: sans;
$button__border-radius--lg: 20px;
```

Element styles
```scss
.button {
    color: $button__color;
    font-family: $button__font-family--sans;
    border-radius: $button__border-radius--lg;

    &:hover {
        color: $button__color--hover;
    }
}
```

### Element with modifier: `.button.button--primary`

HTML
```html
<button class='button button--primary'></button>
```

Sass variables
```scss
$button-primary__color: orange;
$button-primary__color--hover: violet;

```

Element styles
```scss
.button {
    &.button--primary {
        color: $button-primary__color;

        &:hover {
            color: $button-primary__color--hover;
        }
    }
}
```

---
This Sass variable naming convention was originally developed and used within the Kwiziq project, an AI language learning platform. It promotes clear, consistent, and scalable variable naming, and we believe it can be beneficial to other projects as well.

Kwiziq
https://french.kwiziq.com/