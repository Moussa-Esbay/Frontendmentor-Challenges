# My-first-repository
This repository contains a project from frontendmentor.io, it's a QR-code project.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![](./screenshot.jpg)

![Qr-code screenshot](https://github.com/Moussa-Esbay/My-first-repository/assets/137887050/5c5b9548-7d29-4628-a497-aaab9ab05b1b)

### Links!

- Solution URL: [My solution](https://github.com/Moussa-Esbay/My-first-repository)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I learned something new in this project: When I shrink the browser window and my website appears to shrink only on the right side, the solution I found is to Use Relative Units (vh and vw).

Code snippets:

```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>QR code</title>
    <link rel="stylesheet" href="style.css">
    <link rel="shortcut icon" href="imgs/favicon-32x32.png" type="image/x-icon">
</head>

<body>
    <div class="container">
        <div class="qr-code">
            <img src="imgs/image-qr-code.png" alt="Qr-Code" width="280" height="280">
        </div>
        <div class="text">
            <p class="bold">
                Improve your front-end skills by building projects
            </p>
            <p class="light">
                Scan the QR code to visit Frontend Mentor and take your coding skills to the next level
            </p>
        </div>
    </div>
</body>

</html>
```
```css
@import url("https://fonts.googleapis.com/css2?family=Outfit:wght@400;700&display=swap");

/* RESET */

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

/*  */

body {
  background-color: hsl(210, 21%, 93%);
  font-family: "Outfit", sans-serif;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  margin: 10vh 10vw;
}

.container {
  border-radius: 20px;
  padding: 20px 20px 40px 20px;
  width: 320px;
  background-color: hsl(0, 0%, 100%);
}

.qr-code {
  padding-bottom: 30px;
}

.qr-code img {
  border-radius: 20px;
}

p {
  font-size: 15px;
}

.bold {
  font-weight: 700;
  padding-bottom: 20px;
}

.light {
  font-weight: 400;
}

```




### Continued development

I want to practice more, so I should take on more projects.


### Useful resources

- https://www.chat.openai.com - This helps me to figure out the issue mentioned above.
- https://www.fonts.google.com - This help to use a new font.


## Author

- Website - [Moussa]
- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)

## Acknowledgments

I took this challenge by myself, thank you "frontendmentor".
