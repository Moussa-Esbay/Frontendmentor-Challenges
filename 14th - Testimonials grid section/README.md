# Frontend Mentor - Testimonials grid section solution

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

## Overview

### Screenshot

![Desktop-design](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/assets/137887050/37dc93d6-1ca1-4ab2-abff-99b4723dc138)

![Mobile-design](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/assets/137887050/575f1a39-2c21-43e3-9499-51c1255687be)

### Links

- Solution URL: [solution URL](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/tree/main/14th%20-%20Testimonials%20grid%20section)
- Live Site URL: [live site URL](https://6564a91e25d30a51782969c1--scintillating-marigold-a4c12a.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid

To see how you can add code snippets, see below:

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Testimonials grid section</title>
  <link rel="shortcut icon" href="images/favicon-32x32.png" type="image/x-icon">
  <link rel="stylesheet" href="style.css">
</head>

<body>
  <main>
    <section class="daniel-section">
      <figure>
        <img src="images/image-daniel.jpg" alt="Daniel" width="33" height="33">
        <figcaption>
          <span>Daniel Clifford</span>
          <br>
          <span style="color: hsla(0, 0%, 100%, 50%);">Verified Graduate</span>
        </figcaption>
      </figure>
      <h2>I received a job offer mid- course, and the subjects I learned were current, if not more so, in the company I
        joined. I honestly feel I got every penny's worth.</h2>
      <p>"I was an EMT for many years before I joined the bootcamp. I've been looking to make a transition and have
        heard some people who had an amazing experience here.signed up for the free intro course and found it incredibly
        fun! I enrolled shortly thereafter. The next 12 weeks was the best - and most grueling - time of my life. Since
        completing the course, I've successfully switched careers, working as a Software Engineer at a VR startup."</p>
    </section>
    <section class="jonathan-section">
      <figure>
        <img src="images/image-jonathan.jpg" alt="jonathan" width="33" height="33">
        <figcaption>
          <span>Jonathan Walters</span>
          <br>
          <span style="color: hsla(0, 0%, 100%, 50%);">Verified Graduate</span>
        </figcaption>
      </figure>
      <h2>
        The team was very supportive and kept me motivated
      </h2>
      <p>
        "I started as a total newbie with virtually no coding skills. I now work as a mobile engineer for a big company.
        This was one of the best investments l've made in myself."
      </p>
    </section>
    <section class="jeanette-section">
      <figure>
        <img src="images/image-jeanette.jpg" alt="jeanette" width="33" height="33">
        <figcaption>
          <span>Jeanette Harmon</span>
          <br>
          <span style="color: hsla(217, 19%, 35%, 50%);">Verified Graduate</span>
        </figcaption>
      </figure>
      <h2>An overall wonderful and rewarding experience</h2>
      <p>"Thank you for the wonderful experience! I now have a job I really enjoy, and make a good living while doing
        something I love."</p>
    </section>
    <section class="patrick-section">
      <figure>
        <img src="images/image-patrick.jpg" alt="Patrick" width="33" height="33">
        <figcaption>
          <span>Patrick Abrams</span>
          <br>
          <span style="color: hsla(0, 0%, 100%, 50%);">Verified Graduate</span>
        </figcaption>
      </figure>
      <h2>Awesome teaching support from TAs who did the bootcamp themselves. Getting guidance from them and learning
        from their experiences was easy.</h2>
      <p>"The staff seem genuinely concerned about my progress which I find really refreshing. The program gave me the
        confidence necessary to be able to go out in the world and present myself as a capable junior developer. The
        standard is above the rest. You will get the personal attention you need from an incredible community of smart
        and amazing people."</p>
    </section>
    <section class="kira-section">
      <figure>
        <img src="images/image-kira.jpg" alt="Kira" width="33" height="33">
        <figcaption>
          <span>Kira Whittle</span>
          <br>
          <span style="color: hsla(217, 19%, 35%, 50%);">Verified Graduate</span>
        </figcaption>
      </figure>
      <h2>Such a life-changing experience. Highly recommended!</h2>
      <p>"Before joining the bootcamp, l've never written a line of code. I needed some structure from professionals who
        can help me learn programming step by step. I was encouraged to enroll by a former student of theirs who can
        only say wonderful things about the program. The entire curriculum and staff did not disappoint. They were very
        hands-on and I never had to wait long for assistance. The agile team project, in particular, was outstanding. It
        took my learning to the next level in a way that no tutorial could ever have. In fact, l've Often referred to it
        during interviews as an example of my developent experience. It certainly helped me land a job as a full-stack
        developer after receiving multiple offers. 100% recommend!"</p>
    </section>
  </main>
</body>

</html>
```
```css
@import url('https://fonts.googleapis.com/css2?family=Barlow+Semi+Condensed:wght@500;600&display=swap');


:root {
    --MODERATE-VIOLET: hsl(263, 55%, 52%);
    --VERY-DARK-GRAYISH-BLUE: hsl(217, 19%, 35%);
    --VERY-DARK-BLACKISH-BLUE: hsl(219, 29%, 14%);
    --WHITE: hsl(0, 0%, 100%);
    --LIGHT-GRAY: hsl(0, 0%, 81%);
    --LIGHT-GRAYICH-BLUE: hsl(210, 46%, 95%);
}

/* RESET */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* GENERAL STYLES */

body {
    font-family: 'Barlow Semi Condensed', sans-serif;
    background-color: var(--LIGHT-GRAYICH-BLUE);
}

main {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 1110px;
    height: 570px;
    display: grid;
    grid-template-columns: repeat(4, auto);
    grid-template-rows: repeat(2, auto);
    column-gap: 30px;
    row-gap: 30px;
}

section {
    padding: 1.5em;
    border-radius: 10px;
}

img {
    border-radius: 50%;
}

figcaption {
    display: inline-block;
    margin-left: 1em;
}

p,
span {
    font-size: 13px;
}

/* DANIEL */

.daniel-section {
    background-color: var(--MODERATE-VIOLET);
    grid-column: 1 / 3;
    background-image: url(images/bg-pattern-quotation.svg);
    background-repeat: no-repeat;
    background-position: right top;
}

.daniel-section img {
    border: 2px solid hsl(263, 63%, 66%);
}

.daniel-section span:nth-child(1) {
    color: var(--WHITE);
}

.daniel-section h2 {
    margin-top: 1rem;
    color: var(--WHITE);
    font-size: 21px;
}

.daniel-section p {
    margin-top: 1rem;
    color: hsla(0, 0%, 100%, 70%);
}

/* JONATHAN */

.jonathan-section {
    background-color: var(--VERY-DARK-GRAYISH-BLUE);
}

.jonathan-section span:nth-child(1) {
    color: var(--WHITE);
}

.jonathan-section h2 {
    margin-top: 1rem;
    color: var(--WHITE);
    font-size: 21px;
}

.jonathan-section p {
    margin-top: 1rem;
    color: hsla(0, 0%, 100%, 70%);
}

/* JEANETTE */

.jeanette-section {
    background-color: var(--WHITE);
}

.jeanette-section span:nth-child(1) {
    color: hsl(217, 19%, 35%);
}

.jeanette-section h2 {
    margin-top: 1rem;
    color: hsl(217, 19%, 35%);
    font-size: 21px;
}

.jeanette-section p {
    margin-top: 1rem;
    color: hsla(217, 19%, 35%, 70%);
}

/* PATRICK */

.patrick-section {
    background-color: var(--VERY-DARK-BLACKISH-BLUE);
    grid-column: 2 / 4;
}

.patrick-section img {
    border: 2px solid var(--MODERATE-VIOLET);
}

.patrick-section span:nth-child(1) {
    color: var(--WHITE);
}

.patrick-section h2 {
    margin-top: 1rem;
    color: var(--WHITE);
    font-size: 21px;
}

.patrick-section p {
    margin-top: 1rem;
    color: hsla(0, 0%, 100%, 70%);
}

/* KIRA */

.kira-section {
    background-color: var(--WHITE);
    grid-column: 4 / 5;
    grid-row: 1 / 3;
}

.kira-section span:nth-child(1) {
    color: hsl(217, 19%, 35%);
}

.kira-section h2 {
    margin-top: 1rem;
    color: hsl(217, 19%, 35%);
    font-size: 21px;
}

.kira-section p {
    margin-top: 1rem;
    color: hsla(217, 19%, 35%, 70%);
}

/* MEDIA QUERIES */

@media (max-width: 375px) {
    main {
        margin: 1.5em;
        position: unset;
        transform: unset;
        width: unset;
        height: unset;
        display: grid;
        grid-template-columns: 1fr;
        row-gap: 2em;
    }

    .daniel-section {
        grid-column: 1 / 2;
    }

    .jonathan-section {
        grid-column: 1 / 2;
    }

    .jeanette-section {
        grid-column: 1 / 2;
    }

    .patrick-section {
        grid-column: 1 / 2;
    }

    .kira-section {
        grid-column: 1 / 2;
        grid-row: unset;
    }
}
```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)
