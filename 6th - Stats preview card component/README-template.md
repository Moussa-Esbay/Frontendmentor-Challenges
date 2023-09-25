# Frontend Mentor - Stats preview card component solution

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
- [Author](#author)


## Overview

### Screenshot

![](./scr![Desktop-design](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/assets/137887050/dddfde21-d09b-47db-9af3-890b74e313b8)
eenshot.jpg)
![](./screenshot![Mobile-Design](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/assets/137887050/2e920d4c-555b-4488-80f3-10948b202253)
.jpg)


### Links

- Solution URL: [Add solution URL here](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/tree/main/6th%20-%20Stats%20preview%20card%20component)
- Live Site URL: [Add live site URL here](https://6511f4a23b71c01128e94385--ubiquitous-kulfi-312a34.netlify.app/)

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
  <title>Stats Preview Card Components</title>
  <link rel="stylesheet" href="style.css">
  <link rel="shortcut icon" href="images/favicon-32x32.png" type="image/x-icon">
</head>

<body>
  <main>
    <article class="left-side">
      <p class="main-heading">Get <span>insights</span> that help your business grow.</p>
      <p class="main-paragraph">Discover the benefits of data analytics and make better decisions regarding revenue,
        customer experience, and
        overall efficiency.</p>
      <section class="stats">
        <div class="stating">
          <p class="stat">10k+</p>
          <p class="stat-heading">COMPANIES</p>
        </div>
        <div class="stating">
          <p class="stat">314</p>
          <p class="stat-heading">TEMPLATES</p>
        </div>
        <div class="stating">
          <p class="stat">12M+</p>
          <p class="stat-heading">QUERIES</p>
        </div>
      </section>
    </article>
    <article class="right-side">
      <div class="image"></div>
    </article>
  </main>
</body>

</html>
```
```css
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@400;700&family=Lexend+Deca&display=swap");

/* RESET */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* ROOT */

:root {
  --MAIN-BACKGROUND: hsl(233, 47%, 7%);
  --CARD-BACKGROUND: hsl(244, 38%, 16%);
  --ACCENT: hsl(277, 64%, 61%);
  --MAIN-HEADING-AND-STATS: hsl(0, 0%, 100%);
  --MAIN-PARAGRAPH: hsla(0, 0%, 100%, 0.75);
  --STAT-HEADINGS: hsla(0, 0%, 100%, 0.6);
}

/*  */

body {
  background-color: var(--MAIN-BACKGROUND);
}

main {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 1110px;
  height: 440px;
  display: flex;
  flex-direction: row;
}

/* LEFT-SIDE */

.left-side {
  width: 565px;
  background-color: var(--CARD-BACKGROUND);
  padding: 3.5em;
}

.main-heading {
  color: var(--MAIN-HEADING-AND-STATS);
  font-family: "Lexend Deca", sans-serif;
  font-size: 37px;
  font-weight: 600;
  margin-bottom: 1em;
}

span {
  color: var(--ACCENT);
}

.main-paragraph {
  color: var(--MAIN-PARAGRAPH);
  font-family: "Inter", sans-serif;
  font-size: 15px;
  margin-bottom: 3em;
}

.stats {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}

.stat {
  color: var(--MAIN-HEADING-AND-STATS);
  font-family: "Lexend Deca", sans-serif;
  font-weight: 600;
  font-size: 20px;
}

.stat-heading {
  color: var(--MAIN-PARAGRAPH);
  font-family: "Inter", sans-serif;
  font-size: 13px;
}

/* RIGHT-SIDE */

.right-side {
  width: 545px;
  background-image: url(images/image-header-desktop.jpg);
  background-size: cover;
}

.image {
  width: 545px;
  height: 440px;
  background-color: var(--ACCENT);
  opacity: 0.5;
}

/* MEDIA QUERIES */

@media (max-width: 375px) {
  main {
    margin-top: 90px;
    width: 320px;
    height: 780px;
    flex-direction: column-reverse;
  }

  /* LEFT-SIDE */

  .left-side {
    width: 320px;
    height: 540px;
    padding: unset;
    padding-top: 2em;
    text-align: center;
  }

  .stats {
    flex-direction: column;
    align-content: space-between;
  }

  .stating {
    padding-bottom: 1.5em;
  }

  /* RIGHT-SIDE */

  .right-side {
    width: 320px;
    height: 240px;
    background-image: url(images/image-header-mobile.jpg);
    background-size: cover;
  }

  .image {
    width: 320px;
    height: 240px;
  }
}

```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)
