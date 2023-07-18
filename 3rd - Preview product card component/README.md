# 3rd-Preview-product-card-component
Small project talking about a perfume product

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### Screenshot

![desktop-design](https://github.com/Moussa-Esbay/3rd-Preview-product-card-component/assets/137887050/62c5d9b1-f249-4ef9-9ed6-a8ad48a5a5a6)

![mobile-design](https://github.com/Moussa-Esbay/3rd-Preview-product-card-component/assets/137887050/ed49d81a-4d36-41fa-b752-e590a56afb2d)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

To see how you can add code snippets, see below:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<body>
    <main>
        <section class="image-product">
            <img src="imgs/image-product-desktop.jpg" alt="Image Product" width="300" height="450" class="desktop-image">
            <img src="imgs/image-product-mobile.jpg" alt="Image Product" width="340" height="240" class="mobile-image">
        </section>
        <section class="informations">
            <h1 class="type">PERFUME</h1>
            <p class="category">Gabrielle Essence Eau De Parfum</p>
            <p class="uses">A floral, solar and voluptuous interpretation composed by Oliver Polge, Perfumer-Creator for the House of CHANEL.
            </p>
            <p class="price">$149.99 &nbsp;&nbsp;&nbsp; <span>$169.99</span></p>
            <button>
                <i class="fa fa-shopping-cart"></i> 
                &nbsp; Add to Cart
            </button>
            
        </section>
    </main>
</body>
</html>
```
```css
@import url('https://fonts.googleapis.com/css2?family=Fraunces:wght@700&family=Montserrat:wght@500;700&display=swap');

/* RESET */

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/*  */

body{
    background-color:  hsl(30, 38%, 92%);
}

main{
    display: flex;
    justify-content: center;
    width: 600px;
    height: 450px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: white;
    border-radius: 10px;
}

/* IMAGE STYLES */

.mobile-image{
    display: none;
}

.desktop-image{
    border-radius: 10px 0 0 10px;
}

/* .informations class STYLES */

.informations{
    padding: 35px;
}

h1{
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    font-weight: 500;
    letter-spacing: 3px;
    padding-bottom: 2.5vh;
    color: hsl(228, 12%, 48%);
}

.category{
    font-family: 'Fraunces', serif;
    font-size: 30px;
    font-weight: 700;
    line-height: 32px;
    padding-bottom: 4vh;
}

.uses{
    font-family: 'Montserrat', sans-serif;
    font-weight: 500;
    font-size: 14px;
    line-height: 20px;
    padding-bottom: 3.5vh;
    color: hsl(212, 21%, 14%);
}

.price{
    font-family: 'Fraunces', serif;
    font-weight: 700;
    font-size: 30px;
    padding-bottom: 3.5vh;
    color: hsl(158, 52%, 37%);
}

span{
    font-family: 'Montserrat', sans-serif;
    font-weight: 500;
    font-size: 13px;
    text-decoration: line-through;
    color: hsl(228, 12%, 48%);
}

button{
    width: 240px;
    height: 45px;
    border-radius: 10px;
    background-color: hsl(158, 52%, 37%);
    color: white;
    font-size: 14px;
    font-family: 'Montserrat', sans-serif;
    font-weight: 700;
}

/* MEDIA QUERIES */

@media (max-width: 630px){
    main{
        flex-direction: column;
        width: 340px;
        height: 610px;
        justify-content: flex-start;
    }

    .desktop-image{
        display: none;
    }

    .mobile-image{
        display: unset;
        
    }

    .informations{
        padding: 15px;
    }

    button{
        width: 310px;
    }
}
```

### Useful resources

- [Useful fonts](https://www.example.com) - This is the most practical website for people who want to use several fonts (font-family).
- [Useful icons](https://fontawesome.com/search) - This is an amazing website which helped me to find a variety of icons. I'd recommend it to anyone is looking for them.


## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)

