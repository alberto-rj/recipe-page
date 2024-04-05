# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
    - [Shot recap](#short-recap)
    - [Example](#example)
      - [Output](#output)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Your challenge is to build out this recipe page and get it looking as close to the design as possible.

You can use any tools you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go.

### Screenshot

<details>
  <summary>Mobile version</summary>
  <img 
    alt="" 
    src=""
  />
</details>


<details>
  <summary>Desktop version</summary>
  <img 
    alt="" 
    src=""
  />
</details>

### Links

- [Solution](https://www.frontendmentor.io/solutions/responsive-recipe-page-using-css-media-query-UK55_JEHqR)
- [Live Site](https://alberto-rj.github.io/recipe-page/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow

### What I learned

How to use the CSS `counter-reset` and `counter-increment`
 properties and the CSS `counter()` function to customize the style of an `ol` element.

#### Short recap

- `counter-reset` initalize the `count` with `0`
- `counter-increment` increase `1` to `count`
- `counter()` - get the current value of the `count`

#### Example

Suppose we want to style the following `ol` element, which
each `li` child must have the `✅` checkbox before its number:

```html
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```

```css
ol {
  /** 
   * remove the default
   * list style 
   */
  list-style: none;

  /* set 0 to "my-count"  */
  counter-reset: my-count; 
}

li::before {
  /**
   * increase 1 to "my-count" 
   * for each li
   */
  counter-increment: my-count;

  /* ✅ [n] */
  content: "✅ " counter(my-count) " ";
}
```

##### Output

✅ 1 HTML

✅ 2 CSS

✅ 3 JavaScript

### Continued development

It would be nice if I could:

- Implement the design of this challenge without using CSS Media Query.
- Animate each recipe section when the user is scrolling on the page.

### Useful resources

- [W3Schools](https://www.w3schools.com/cssref/pr_gen_counter-increment.php) - here is where I've learned how to work with `counter-reset`, `counter-increment` and `count()`.

## Author

- Github - [Alberto Raúl José](https://github.com/alberto-rj)
- Frontend Mentor - [@alberto-rj](https://www.frontendmentor.io/profile/alberto-rj)
- Twitter - [@albertorauljose](https://www.twitter.com/yourusername)
