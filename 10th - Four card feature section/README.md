# Frontend Mentor - Four card feature section solution

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot


### Links

- Solution URL: [Solution URL]()
- Live Site URL: [Live site URL]()

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

To see how you can add code snippets, see below:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Four card feature section</title>
    <link rel="shortcut icon" href="images/favicon-32x32.png" type="image/x-icon">
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <p class="first">Reliable, efficient delivery</p>
        <p class="second">Powered by Technology</p>
        <p class="third">Our Artificial intelligence powered tools usw millions project data <br> points to ensure that
            your project
            is
            successful</p>
    </header>
    <main>
        <section class="supervisor">
            <h3>Supervisor</h3>
            <p>Monitors activity to identify project roadblocks</p>
            <img src="images/icon-supervisor.svg" alt="">
        </section>

        <section class="team-builder">
            <h3>Team Builder</h3>
            <p>Scans our talent network to create the optimal team for your project</p>
            <img src="images/icon-team-builder.svg" alt="">
        </section>

        <section class="karma">
            <h3>Karma</h3>
            <p>Regularly evaluates our talent to ensure quality</p>
            <img src="images/icon-karma.svg" alt="">
        </section>

        <section class="calculator">
            <h3>Calculator</h3>
            <p>Uses data from past projects to provide better delivery estimates</p>
            <img src="images/icon-calculator.svg" alt="">
        </section>
    </main>
</body>

</html>
```
```css
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200;400;600&display=swap");

/* RESET */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/*  */

body {
  font-family: "Poppins", sans-serif;
  width: 1120px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  margin-top: -2em;
}

/* HEADER */

header {
  text-align: center;
  margin-top: -20em;
  position: absolute;
  left: 50%;
  transform: translate(-50%, -0%);
}

.first {
  font-size: 30px;
  font-weight: 200;
}

.second {
  color: hsl(234, 12%, 34%);
  font-size: 30px;
  font-weight: 600;
}

.third {
  margin-top: 1em;
  font-size: 15px;
  font-weight: 200;
}

/* MAIN */

section {
  width: 350px;
}

.supervisor {
  position: absolute;
  transform: translate(-0%, -0%);
  border-top: 4px solid hsl(180, 62%, 55%);
  border-radius: 5px;
  padding: 2em;
  background-color: hsl(0, 0%, 98%);
  box-shadow: 0 0 1em hsl(229, 6%, 66%);
}

.team-builder {
  position: absolute;
  top: 50%;
  left: 40%;
  transform: translate(-18%, -50%);
  border-top: 4px solid hsl(0, 78%, 62%);
  border-radius: 5px;
  padding: 2em;
  background-color: hsl(0, 0%, 98%);
  box-shadow: 0 0 1em hsl(229, 6%, 66%);
}

.karma {
  position: absolute;
  top: -50%;
  left: 50%;
  transform: translate(-50%, 50%);
  border-top: 4px solid hsl(34, 97%, 64%);
  border-radius: 5px;
  padding: 2em;
  margin-top: 2em;
  background-color: hsl(0, 0%, 98%);
  box-shadow: 0 0 1em hsl(229, 6%, 66%);
}

.calculator {
  position: absolute;
  left: 100%;
  transform: translate(-100%, -0%);
  border-top: 4px solid hsl(212, 86%, 64%);
  border-radius: 5px;
  padding: 2em;
  background-color: hsl(0, 0%, 98%);
  box-shadow: 0 0 1em hsl(229, 6%, 66%);
}

h3 {
  margin-bottom: 1em;
}

section p {
  font-size: 14px;
  font-weight: 200;
  margin-bottom: 1em;
}

img {
  float: right;
}

/* MEDIA QUERIES */

@media (max-width: 375px) {
  body {
    width: 310px;
    margin-top: unset;
  }

  header {
    position: unset;
    transform: unset;
    margin-top: 36em;
    margin-bottom: 2em;
  }

  .first,
  .second {
    font-size: 24px;
  }

  .supervisor,
  .team-builder,
  .karma,
  .calculator {
    position: unset;
    transform: unset;
    margin-bottom: 2em;
    height: 225px;
    width: 310px;
  }
}

```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)


