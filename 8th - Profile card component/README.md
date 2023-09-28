# Frontend Mentor - Profile card component solution

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
- [Author](#author)

## Overview

### Screenshot

![Desktop-design](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/assets/137887050/f0f3c644-a77d-4199-ae42-3a0befc39c34)

![Mobile-design](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/assets/137887050/a8e28f9d-28da-471f-9080-40b666af1c49)

### Links

- Solution URL: [solution URL](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/tree/main/8th%20-%20Profile%20card%20component)
- Live Site URL: [live site URL](https://6515eba0f011f6057d4ad805--cute-cocada-9882a2.netlify.app/)

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
    <title>Profile card component</title>
    <link rel="shortcut icon" href="images/favicon-32x32.png" type="image/x-icon">
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <main>
        <img src="svgs/bg-pattern-card.svg" alt="" class="pattern-card">
        <img src="images/image-victor.jpg" alt="" class="profil-image">
        <h3 class="name">Victor Crest <span>26</span></h3>
        <p class="city">London</p>
        <hr>
        <section class="stats">
            <div class="stat followers-stat">
                <h3 class="number followers-number">80K</h3>
                <p class="text followers-text">Followers</p>
            </div>
            <div class="stat likes-stat">
                <h3 class="number likes-number">803K</h3>
                <p class="text likes-text">Likes</p>
            </div>
            <div class="stat photos-stat">
                <h3 class="number photos-number">1.4K</h3>
                <p class="text photos-text">Photos</p>
            </div>
        </section>
    </main>
</body>

</html>
```
```css
@import url("https://fonts.googleapis.com/css2?family=Kumbh+Sans:wght@400;700&display=swap");

/* RESET */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/*  */

body {
  font-family: "Kumbh Sans", sans-serif;
  background-color: hsl(185, 75%, 39%);
  background-image: /* url(svgs/bg-pattern-top.svg), */ url(svgs/bg-pattern-bottom.svg);
  background-repeat: no-repeat;
}

main {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 350px;
  height: 380px;
  border-radius: 15px;
  background-color: white;
}

.profil-image {
  position: absolute;
  top: 37%;
  left: 50%;
  transform: translate(-50%, -50%);
  border: 5px solid white;
  border-radius: 50%;
}

.pattern-card {
  border-top-right-radius: 15px;
  border-top-left-radius: 15px;
}

.name {
  margin-top: 3em;
  margin-bottom: 0.3em;
  text-align: center;
  font-size: 18px;
}

span {
  color: hsl(0, 0%, 59%);
}

.city {
  color: hsl(0, 0%, 59%);
  text-align: center;
}

hr {
  margin: 2em 1em 0 1em;
}

.stats {
  display: flex;
  justify-content: space-evenly;
  margin-top: 1.5em;
}

.number {
  font-size: 18px;
}

.text {
  margin-top: 0.3em;
  font-size: 12px;
  color: hsl(0, 0%, 59%);
}

/* MEDIA QUERIES */

@media (max-width: 375px) {
  main {
    width: 330px;
    height: 370px;
  }

  .pattern-card {
    width: 330px;
  }
}

```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)
