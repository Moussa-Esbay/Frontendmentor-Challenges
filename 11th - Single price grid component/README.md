# Frontend Mentor - Single price grid component solution

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

![](./screenshot.jpg)



### Links

- Solution URL: [solution URL]()
- Live Site URL: [live site URL]()

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
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
    <title>Single price grid component</title>
    <link rel="stylesheet" href="style.css" />
    <link
      rel="shortcut icon"
      href="images/favicon-32x32.png"
      type="image/x-icon"
    />
  </head>
  <body>
    <main>
      <section class="join-us">
        <h1>Join our community</h1>
        <h2>30-day, hassle-free money back guaantee</h2>
        <p>
          Gain access to our full library of tutorials along with expert code
          reviews. Perfect for any developers who are serious about haning their
          skills.
        </p>
      </section>
      <section class="subscription">
        <h2>Monthly Subscription</h2>
        <p><span>$29</span> <span>per month</span></p>
        <p>Full access for less than $1 a day</p>
        <button>Sign Up</button>
      </section>
      <section class="why-us">
        <h2>Why Us</h2>
        <ul>
          <li>Tutorials by industry experts</li>
          <li>Peer & expert code review</li>
          <li>Coding exercises</li>
          <li>Access to our GitHub repos</li>
          <li>Community forum</li>
          <li>Flahcard decks</li>
          <li>New videos every week</li>
        </ul>
      </section>
    </main>
  </body>
</html>

```
```css
@import url("https://fonts.googleapis.com/css2?family=Karla:wght@400;700&display=swap");

/* RESET */

* {
  margin: 0;
  padding: 0;
  box-sizing: 0;
}

/* MAIN */

body {
  font-family: "Karla", sans-serif;
  background-color: hsl(204, 43%, 93%);
}

main {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 640px;
  display: grid;
  grid-template-columns: 1fr 1fr;
}

/* 1st section */
.join-us {
  background-color: white;
  padding: 2em;
  grid-column: 1 / 3;
}

h1 {
  color: hsl(179, 62%, 43%);
  font-size: 20px;
  margin-bottom: 1em;
}

.join-us h2 {
  color: hsl(71, 73%, 54%);
  font-size: 15px;
  line-height: 1em;
  margin-bottom: 1em;
}

.join-us p {
  font-size: 16px;
  color: rgb(181, 181, 181);
  line-height: 2em;
}

/* 2nd section */
.subscription {
  background-color: hsl(179, 55%, 49%);
  padding: 1em;
  color: white;
}

.subscription h2 {
  font-size: 18px;
}

span:first-child {
  font-size: 30px;
}

span:nth-child(2) {
  color: hsl(204, 43%, 93%);
}

button {
  margin-top: 2em;
  position: relative;
  left: 50%;
  transform: translate(-50%);
  background-color: hsl(71, 73%, 54%);
  color: white;
  border: unset;
  border-radius: 10px;
  padding: 1.5em 9em;
  text-wrap: nowrap;
}

/* 3rd section */
.why-us {
  background-color: hsl(179, 60%, 52%);
  padding: 1em;
}

.why-us h2 {
  color: white;
  font-size: 17px;
  margin-bottom: 1em;
}

li {
  list-style: none;
  color: rgb(244, 244, 244);
  font-size: 15px;
  line-height: 1.5em;
}

/* MEDIA QUERIES */
@media (max-width: 675px) {
  body {
    height: 820px;
  }

  main {
    width: 310px;
    position: absolute;
    left: 50%;
    top: unset;
    transform: translate(-50%);
    border-radius: 10px;
    margin-top: 1em;
    display: unset;
  }

  /* 1st section */
  .join-us {
    padding: 1em;
  }

  h1 {
    color: hsl(179, 62%, 43%);
    font-size: 20px;
    margin-bottom: 1em;
  }

  .join-us h2 {
    color: hsl(71, 73%, 54%);
    font-size: 15px;
    line-height: 1em;
    margin-bottom: 1em;
  }

  .join-us p {
    font-size: 16px;
    color: rgb(181, 181, 181);
    line-height: 2em;
  }

  /* 2nd section */
  .subscription {
    padding: 1em;
    color: white;
  }

  .subscription h2 {
    font-size: 18px;
  }

  span:first-child {
    font-size: 30px;
  }

  span:nth-child(2) {
    color: hsl(204, 43%, 93%);
  }

  button {
    margin-top: 2em;
    position: relative;
    left: 50%;
    transform: translate(-50%);
    background-color: hsl(71, 73%, 54%);
    color: white;
    border: unset;
    border-radius: 10px;
    padding: 1.5em 9em;
    text-wrap: nowrap;
  }

  /* 3rd section */
  .why-us {
    padding: 1em;
  }

  .why-us h2 {
    color: white;
    font-size: 17px;
    margin-bottom: 1em;
  }

  li {
    list-style: none;
    color: rgb(244, 244, 244);
    font-size: 15px;
    line-height: 1.5em;
  }
}

```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)

