# The Odin Project - Project: Admin Dashboard

This is a solution to the [Project: Admin Dashboard on Odin](https://www.theodinproject.com/lessons/node-path-intermediate-html-and-css-admin-dashboard). 

## Overview

A full dashboard design using CSS Grid and Flexbox

### Screenshot

![](./assets/Screen%20Shot%202022-07-04%20at%2010.28.57%20AM.png)

### Links

- Live Site URL: [https://selt0.github.io/admin-dashboard/](https://selt0.github.io/admin-dashboard/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- [Material Design Icons](https://materialdesignicons.com/) - For icons

### What I learned

I used CSS variables to make it easy to change the color theme in the future. I used CSS Grid to create the layout of columns and rows while using Flexbox to postition the elements within the column or rows.

```css

:root {
    --light-blue: #1992d4;
    --gold: #f0b429;
    --gray: #e2e8f0;
    --text: #636363
}

body {
    display: grid;
    grid-template-columns: clamp(200px, 250px, 300px) 3fr clamp(200px, 250px, 300px);
    grid-template-rows: 150px 4fr;
    height: 100vh;
    font-family: 'Roboto', sans-serif;
    font: 16px;
}

header {
    grid-column: 2 / 4;
    display: grid;
    grid-template-columns: 2fr minmax(320px, 1fr);
    grid-template-rows: 1fr 1fr;
    align-items: center;
    padding-left: 25px;
}

.side-bar {
    grid-row: 1 / 3;
    background: var(--light-blue);
    color: #fff;
    display: flex;
    flex-direction: column;
}
```

### Continued development

Before I was under the impression to use either Flexbox or Grid to create layouts and position elements. With this project, I realize that Grid isn't meant to replace flexbox but instead be used as another tool to create layouts. CSS Grid is perfect for creating layouts with rows AND columns whereas Flexbox is used to position the elements within the row OR column.

### Useful resources

- [Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - This helped me have a quick reference to Grid properties

## Author

- Website - [Michael Martinez](https://michael-martinez.netlify.app/)
- Twitter - [@MMocomochi](https://twitter.com/MMocomochi)