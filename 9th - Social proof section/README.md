# Frontend Mentor - Social proof section solution

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
- [Author](#author)

## Overview

### Screenshot
![Desktop-design](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/assets/137887050/866ba369-acc1-4132-b1b2-b0df670c9824)

![Mobile-design](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/assets/137887050/b1577240-4639-4757-96ce-6ccd8ca52c81)

### Links

- Solution URL: [solution URL](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/tree/main/9th%20-%20Social%20proof%20section)
- Live Site URL: [live site URL](https://651e906b04faee08931dc86c--polite-dusk-2c7c1d.netlify.app/)

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
    <title>Social proof section</title>
    <link rel="shortcut icon" href="images/favicon-32x32.png" type="image/x-icon">
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <main>
        <section class="stat">
            <h1>10,000+ of our users love our products.</h1>
            <p class="stat-text">We only provide great products combined with excellent customer service. See what our
                satisfied customers
                are
                saying about our services.</p>
        </section>
        <section class="rating">
            <div class="rate first-rate">
                <div>
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                </div>
                <p>Rated 5 Stars in Reviews</p>
            </div>
            <div class="rate second-rate">
                <div>
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                </div>
                <p>Rated 5 Stars in Report Guru</p>
            </div>
            <div class="rate third-rate">
                <div>
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                    <img src="images/icon-star.svg" alt="" class="star-icon">
                </div>
                <p>Rated 5 Stars in BestTech</p>
            </div>
        </section>
        <section class="opinions">
            <div class="card colton">
                <figure>
                    <img src="images/image-colton.jpg" alt="" class="picture">
                    <figcaption>Colton Smith <span>Verified Buyer</span></figcaption>
                </figure>
                <p>"We needed the same printed design as the one we had ordered a week prior. Not only did they find the
                    original order, but we also received it in time. Excellen!"</p>
            </div>
            <div class="card irene">
                <figure>
                    <img src="images/image-irene.jpg" alt="" class="picture">
                    <figcaption>Irene Roberts <span>Verified Buyer</span></figcaption>
                </figure>
                <p>"Customer service is always excellent and very quick turn around. Completely
                    delighted with the
                    simplicity of the purchase and the speed of delivery."</p>
            </div>
            <div class="card anne">
                <figure>
                    <img src="images/image-anne.jpg" alt="">
                    <figcaption>Anne Wallace <span>Verified Buyer</span></figcaption>
                </figure>
                <p>"Put an order with this company and can only praise them for the ver high standard. Will definitely
                    use them again and recommend them to everyone! "</p>
            </div>
        </section>
    </main>
</body>

</html>
```
```css
@import url("https://fonts.googleapis.com/css2?family=League+Spartan:wght@400;500;700&display=swap");

/* RESET */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/*  */

body {
  font-family: "League Spartan", sans-serif;
  background-image: url(images/bg-pattern-bottom-desktop.svg),
    url(images/bg-pattern-top-desktop.svg);
  background-repeat: no-repeat, no-repeat;
}

main {
  width: 1110px;
  height: 585px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

/* CLASS = "STAT" */

h1 {
  width: 335px;
  font-size: 40px;
  color: hsl(300, 43%, 22%);
  margin-bottom: 0.6em;
}

.stat-text {
  width: 405px;
  color: hsl(303, 10%, 53%);
  font-weight: 500;
  font-size: 17px;
  line-height: 1.2em;
}

/* CLASS = "RATING" */

.rating {
  float: right;
  margin-top: -11em;
  max-width: 450px;
}

.rating div {
  display: flex;
}

.star-icon {
  padding-right: 0.2em;
}

.rate {
  background-color: hsl(300, 24%, 96%);
  border-radius: 10px;
  padding: 1em;
  margin-bottom: 1em;
  justify-content: center;
}

.first-rate {
  margin-left: -4em;
  margin-right: 4em;
}

.second-rate {
  margin-left: -2em;
  margin-right: 2em;
}

.rating p {
  padding-left: 1.5em;
  padding-right: 1em;
  color: hsl(300, 43%, 22%);
  font-weight: 900;
}

/* CLASS = "OPINIONS" */

.opinions {
  margin-top: 2em;
  display: flex;
  justify-content: space-between;
}

.card {
  width: 350px;
  background-color: hsl(300, 43%, 22%);
  border-radius: 5px;
  padding: 2em;
}

.card figure {
  margin-bottom: 2em;
  display: flex;
}

.card img {
  width: 40px;
  border-radius: 50%;
  margin-right: 1em;
}

.card figcaption {
  color: hsl(0, 0%, 100%);
  margin-top: 0.3em;
}

span {
  display: block;
  color: hsl(333, 80%, 67%);
  margin-top: 0.2em;
}

.card p {
  color: hsl(0, 0%, 100%);
  font-size: 15px;
  line-height: 1.5em;
  font-weight: 500;
}

.irene {
  margin-top: 1em;
  margin-bottom: -1em;
}

.anne {
  margin-top: 2em;
  margin-bottom: -2em;
}

/* MEDIA QUERIES */

@media (max-width: 375px) {
  body {
    background-image: url(images/bg-pattern-bottom-mobile.svg),
      url(images/bg-pattern-top-mobile.svg);
    background-repeat: no-repeat, no-repeat;
  }

  main {
    width: 315px;
  }

  .stat {
    text-align: center;
    margin-bottom: 2em;
  }

  .stat-text {
    width: unset;
  }

  .rating {
    float: unset;
    margin: unset;
    text-align: center;
  }

  .first-rate,
  .second-rate {
    margin: unset;
    margin-bottom: 0.8em;
  }

  .rate {
    flex-direction: column;
    align-items: center;
  }

  .rating p {
    padding: unset;
    padding-top: 0.8em;
  }

  .opinions {
    flex-direction: column;
  }

  .card {
    width: unset;
  }
}

```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)
