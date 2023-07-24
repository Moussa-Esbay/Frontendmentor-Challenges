# 5th - Order summary component

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
- [Author](#author)

### Screenshot




### Links

- Solution URL: [solution URL](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/tree/main/5th%20-%20Order%20summary%20component)
- Live Site URL: [live site URL](https://64bea8fb9fdbb11bdf6db682--neon-tulumba-9d7c69.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties

To see how you can add code snippets, see below:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Order summary component</title>
    <link rel="stylesheet" href="style.css">
    <link rel="shortcut icon" href="images/favicon-32x32.png" type="image/x-icon">
</head>
<body>
    <main>
        <img src="svgs/illustration-hero.svg" alt="Hero" width="450" height="220" class="hero">
        <h1>Order Summary</h1>
        <p>You can now listen to millions of songs, audiobooks, and podcasts on any device anywhere you like!</p>
        <section>
            <img src="svgs/icon-music.svg" alt="music-icon">
            <p>
                <span class="text">Annual Plan</span>
                <br>
                <span class="price">$59.99/year</span>
            </p>
            <a href="" class="change">Change</a>
        </section>
        <button type="button" onclick="alert('Payment successed')">Proceed to Payment</button>
        <a href="" class="cancel">Cancel Order</a>
    </main>
</body>
</html>
```
```css
@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Display:wght@500;700;900&display=swap');

/* RESET */

*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

/*  */

body{
    background-image: url('svgs/pattern-background-desktop.svg');
    background-repeat: no-repeat;
    background-size: cover;
    background-color:   hsl(225, 100%, 98%);
}

main{
    width: 450px;
    height: 700px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    font-family: 'Red Hat Display', sans-serif;
    background-color: hsl(0, 0%, 100%);
    border-radius: 30px;
}

.hero{
    border-radius: 30px 30px 0 0 ;
}

h1{
    margin-top: 1.3em;
    font-size: 28px;
    font-weight: 900;
}

p{
   margin-top: 1.2em; 
   font-size: 16px;
   font-weight: 500;
   margin-left: 3em;
   margin-right: 3em;
   line-height: 1.5em;
   color: hsl(224, 23%, 55%);
}

section{
    height: 85px;
    margin: 1em 3em 2em 3em;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: hsl(225, 100%, 98%);
    border-radius: 20px;
}

p span{
    margin-left: -2em;
    margin-right: 3em;
}

.text{
    font-weight: 900;
    color: black;
}

.price{
    font-weight: 500;
    color: hsl(224, 23%, 55%);
}

.change{
    font-size: 13px;
    font-weight: 900;
    color: hsl(245, 75%, 52%);
}

button{
    display: block;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 2.5em;
    width: 350px;
    height: 50px;
    border-radius: 10px;
    border: none;
    background-color:hsl(245, 75%, 52%);
    color: hsl(0, 0%, 100%);
    font-size: 15px;
    font-weight: 900;
    word-spacing: 2px;
    font-family: 'Red Hat Display', sans-serif;
    box-shadow: 0 30px 0 0 hsl(225, 100%, 98%);
}

button:hover{
    cursor: pointer;
    scale: 1.025;
}

.cancel{
    text-decoration: none;
    font-weight: 900;
    color: hsl(224, 23%, 55%);
    font-size: 15px;
}

/* MEDIA QUERIES */

@media (max-width: 460px){
    body{
    background-image: url('svgs/pattern-background-mobile.svg');
    background-repeat: no-repeat;
    background-size: cover;
    }

    main{
        width: 330px;
        height: 570px;
    }

    .hero{
        width: 330px;
    }

    p span{
        font-size: 14px;
        margin: unset;
        margin-left: -2em;
        margin-right: -2em;
    }
}
```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)

