# Frontend Mentor - Huddle landing page with single introductory section solution

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

- Solution URL: [solution URL]()
- Live Site URL: [live site URL]()

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

To see how you can add code snippets, see below:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Huddle landing page with a single introductory section</title>
    <link rel="stylesheet" href="style.css" />
    <link
      rel="shortcut icon"
      href="images/favicon-32x32.png"
      type="image/x-icon"
    />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css"
    />
  </head>
  <body>
    <main>
      <article>
        <section>
          <img src="images/logo.svg" alt="Logo" width="220" class="logo" />
          <img
            src="images/illustration-mockups.svg"
            alt="Illustration"
            width="590"
            height="420"
            class="illustration"
          />
        </section>
        <section>
          <h1>Build The Community Your Fans Will Love</h1>
          <p>
            Huddle re-imagines the way we build communities. You have a voice,
            but so does your audience. Create connections with your users as you
            engage in genuine discussion.
          </p>
          <button>Register</button>
        </section>
      </article>
      <ul>
        <li><i class="fa-brands fa-facebook-f"></i></li>
        <li><i class="fa-brands fa-twitter"></i></li>
        <li><i class="fa-brands fa-instagram"></i></li>
      </ul>
    </main>
  </body>
</html>

```
```css
@import url("https://fonts.googleapis.com/css2?family=Open+Sans&family=Poppins:wght@400;600&display=swap");

/* RESET */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* GENERAL */

body {
  background-color: hsl(257, 40%, 49%);
  background-image: url(images/bg-desktop.svg);
}

main {
  width: 1270px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
}

article {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

.illustration {
  width: 700px;
  height: 490px;
  margin-right: 4em;
  margin-top: 5em;
}

section:nth-child(2) {
  margin-top: 12em;
}

h1 {
  font-family: "Poppins", sans-serif;
  font-size: 40px;
  margin-bottom: 0.7em;
}

p {
  font-family: "Open Sans", sans-serif;
  font-size: 20px;
  margin-bottom: 1em;
}

button {
  margin-bottom: 4em;
  padding: 0.7em 4em;
  border-radius: 50px;
  font-size: 20px;
  font-weight: 500;
  color: hsl(257, 40%, 49%);
  border: unset;
}

button:hover {
  background-color: hsl(300, 69%, 71%);
  cursor: pointer;
  color: white;
}

li:hover {
  border: 2px solid hsl(300, 78%, 53%);
  cursor: pointer;
}

i:hover {
  color: hsl(300, 78%, 53%);
}

ul {
  list-style-type: none;
  display: flex;
  justify-content: flex-end;
  gap: 1.5em;
}

li {
  border: 2px solid white;
  border-radius: 50%;
  padding: 0.5em;
  font-size: 20px;
}

/* MEDIA QUERIES */
@media (max-width: 750px) {
  body {
    background-image: url(images/bg-mobile.svg);
    background-repeat: no-repeat;
    background-size: cover;
  }

  main {
    margin-top: 2em;
    height: 1260px;
    width: 590px;
    position: absolute;
    left: 50%;
    top: unset;
    transform: translate(-50%);
    color: white;
  }

  article {
    display: unset;
  }

  .logo {
    margin-bottom: 4em;
  }

  .illustration {
    margin-bottom: 4em;
    margin-right: unset;
    margin-top: unset;
    width: 590px;
    height: 420px;
  }

  section:nth-child(2) {
    margin-top: unset;
  }

  h1 {
    font-family: "Poppins", sans-serif;
    font-size: 52px;
    margin-bottom: 0.7em;
  }

  h1,
  p,
  ul {
    text-align: center;
  }

  p {
    font-family: "Open Sans", sans-serif;
    font-size: 30px;
    margin-bottom: 1em;
  }

  button {
    position: relative;
    left: 50%;
    transform: translate(-50%);
    margin-bottom: 4em;
    padding: 1em 5em;
    border-radius: 50px;
    font-size: 16px;
    font-weight: 500;
    color: hsl(257, 40%, 49%);
  }

  ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
    gap: 1.5em;
  }

  li {
    border: 2px solid white;
    border-radius: 50%;
    padding: 0.5em;
    font-size: 20px;
  }
}

```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)
