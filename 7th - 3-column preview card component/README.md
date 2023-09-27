# Frontend Mentor - 3-column preview card component solution

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
- [Author](#author)

## Overview

### Screenshot



### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

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
    <title>3-column preview card component</title>
    <link rel="stylesheet" href="style.css">
    <link rel="shortcut icon" href="icon/favicon-32x32.png" type="image/x-icon">
</head>

<body>
    <main>
        <section class="sedans">
            <img src="svgs/icon-sedans.svg" alt="Sedans" class="sedans-svg">
            <h1 class="sedans-heading">SEDANS</h1>
            <p class="sedans-paragraph">Choose a sedan for its affordability and excellent fuel economy. Ideal for
                cruising in the city or on
                your next road trip.</p>
            <button class="sedans-button">Learn More</button>
        </section>
        <section class="suvs">
            <img src="svgs/icon-suvs.svg" alt="Suvs" class="suvs-svg">
            <h1 class="suvs-heading">SUVS</h1>
            <p class="suvs-paragraph">Take an SUV for its spacious interior, power, and versality.Perfect for you next
                family vacation and
                off-road adventures.</p>
            <button class="suvs-button">Learn More</button>
        </section>
        <section class="luxury">
            <img src="svgs/icon-luxury.svg" alt="Luxury" class="luxury-svg">
            <h1 class="luxury-heading">LUXURY</h1>
            <p class="luxury-paragraph">Cruise in the best car brands without the bloated prices.Enjoy the enhaced
                comfort of a luxury rental and
                arrive in style.</p>
            <button class="luxury-button">Learn More</button>
        </section>
    </main>
</body>

</html>
```
```css
@import url("https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@700&family=Lexend+Deca&display=swap");

:root {
  --BRIGHT-ORANGE: hsl(31, 77%, 52%);
  --DARK-CYAN: hsl(184, 100%, 22%);
  --VERY-DARK-CYAN: hsl(179, 100%, 13%);
  --PARAGRAPHS: hsla(0, 0%, 100%, 0.75);
  --BACKGROUND-HEADINGS-BUTTONS: hsl(0, 0%, 95%);
}

/* RESET */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* GENERAL STYLES */

body {
  background-color: var(--BACKGROUND-HEADINGS-BUTTONS);
}

main {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 930px;
  height: 500px;
  display: flex;
}

section {
  padding: 2em;
}

img {
  margin-bottom: 2em;
}

h1 {
  color: var(--BACKGROUND-HEADINGS-BUTTONS);
  font-family: "Big Shoulders Display", cursive;
  margin-bottom: 2em;
  font-size: 35px;
}

p {
  font-size: 15px;
  color: var(--PARAGRAPHS);
  font-family: "Lexend Deca", sans-serif;
  line-height: 1.7em;
  margin-bottom: 3em;
  height: 130px;
}

button {
  background-color: var(--BACKGROUND-HEADINGS-BUTTONS);
  border: unset;
  font-family: "Big Shoulders Display", cursive;
  font-size: 15px;
  letter-spacing: 0.1em;
  padding: 1em 2em;
  border-radius: 30px;
}

/* SEDANS SECTION */

.sedans {
  background-color: var(--BRIGHT-ORANGE);
  border-bottom-left-radius: 5px;
  border-top-left-radius: 5px;
}

.sedans-button {
  color: var(--BRIGHT-ORANGE);
}

/* SUVS SECTION */

.suvs {
  background-color: var(--DARK-CYAN);
}

.suvs-button {
  color: var(--DARK-CYAN);
}

/* LUXURY SECTION */

.luxury {
  background-color: var(--VERY-DARK-CYAN);
  border-top-right-radius: 5px;
  border-bottom-right-radius: 5px;
}

.luxury-button {
  color: var(--VERY-DARK-CYAN);
}

/* MEDIA-QUERIES */

@media (max-width: 375px) {
  main {
    width: 330px;
    flex-direction: column;
    top: 45%;
  }

  p {
    height: 100px;
  }

  /* SEDANS SECTION */

  .sedans {
    height: 450px;
    border-top-right-radius: 5px;
    border-top-left-radius: 5px;
  }

  /* SUVS SECTION */

  .suvs {
    height: 450px;
  }

  /* LUXURY SECTION */

  .luxury {
    height: 450px;
    border-bottom-right-radius: 5px;
    border-bottom-left-radius: 5px;
  }
}

```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)

