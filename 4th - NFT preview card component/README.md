4th-NFT-Preview-card-component
 
 ## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
- [Author](#author)


## Overview

### Screenshot

![NFT preview card screenshot](https://github.com/Moussa-Esbay/Frontendmentor-Challenges/assets/137887050/a497321e-2815-46ff-992c-d2a1d57260d4)

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
    <title>NFT preview card component</title>
    <link rel="stylesheet" href="style.css">
    <link rel="shortcut icon" href="images/favicon-32x32.png" type="image/x-icon">
</head>
<body>
    <main>
        <section>
        <img src="images/image-equilibrium.jpg" alt="Equilibrium" class="equilibrium" width="300" height="300">
        <h1>Equilibrium #3429</h1>
        <p class="description">Our Equilibrium collection promotes balance and calm</p>
        <p>
            <span class="ethereum">
                <img src="svgs/icon-ethereum.svg" alt="Ethereum">&nbsp;
                0.041 ETH
            </span>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            <span class="clock">
                <img src="svgs/icon-clock.svg" alt="Clock">&nbsp;
                3 days left
            </span>
        </p>
        <div>
            <img src="images/image-avatar.png" alt="Avatar" class="avatar" width="35" height="35">
            <p class="creator">
                <span>Creation of</span> 
                <span class="name">Jules Wyvern</span>
            </p>
        </div>
    </section>
    </main>
</body>
</html>
```
```css
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600&display=swap');

/* RESET */

*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

/*  */

body{
    background-color: hsl(217, 54%, 11%) ;
}

main{
    font-family: 'Outfit', sans-serif;
    width: 350px;
    height: 600px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: hsl(216, 50%, 16%);
    border-radius: 5px;
}

section{
    margin-left: 1.6em;
}

.equilibrium{
    /* display: block;
    margin-left: auto;
    margin-right: auto; */
    margin-top: 1.5em;
    margin-bottom: 0.7em;
}

h1{
    font-size: 23px;
    color: hsl(0, 0%, 100%);
}

.description{
    font-size: 18px;
    line-height: 1.4em;
    color: hsl(215, 51%, 70%);
    margin-bottom: 1em;
}

.ethereum{
    color: hsl(178, 100%, 50%);
    font-weight: 600;
}

.clock{
    color: hsl(215, 51%, 70%);
    font-weight: 600;
}

div{
    display: flex;
    margin-top: 1.6em;
}

.avatar{
    border: 1px solid hsl(0, 0, 100%);
}

.creator{
    margin-left: 1em;
}

.creator:nth-child(2){
    color: hsl(215, 51%, 70%);
}

.name{
    color: hsl(0, 0%, 100%);
}


```

## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)
