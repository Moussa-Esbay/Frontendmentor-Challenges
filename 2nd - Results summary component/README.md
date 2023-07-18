# 2nd---Results-summary-component
Another project from frontendmentor.io (Result - Summary).

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
- [Author](#author)


## Overview

### Screenshot

![My solution's screenshot](https://github.com/Moussa-Esbay/2nd---Results-summary-component/assets/137887050/27684304-c8da-4990-95da-9d1804412f61)

### Links

- Solution URL: [URL's solution](https://github.com/Moussa-Esbay/2nd---Results-summary-component)

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
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <main>
        <section class="result">
            <h2 class="result-head">Your Result</h2>
            <p class="circle"><span class="seventy-six">76</span>of 100</p>
            <p class="great">Great</p>
            <p class="score">You scored higher than 65% of the people who have taken these
                tests.</p>
        </section>
        <section class="summary">
            <h2 class="summary-head">Summary</h2>
            <div class="reaction">
                <img src="svgs/icon-reaction.svg" alt="Reaction">
                <p class="power"><b style="color: hsl(0, 100%, 67%);">Reaction</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <b>80</b> / 100</p>
            </div>
            <div class="memory">
                <img src="svgs/icon-memory.svg" alt="Memory">
                <p class="power"><b style="color: hsl(39, 100%, 56%);">Memory</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <b>92</b> / 100</p>
            </div>
            <div class="verbal">
                <img src="svgs/icon-verbal.svg" alt="Verbal">
                <p class="power"><b style="color: hsl(166, 100%, 37%);">Verbal</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <b>61</b> / 100</p>
            </div>
            <div class="visual">
                <img src="svgs/icon-visual.svg" alt="Visual">
                <p class="power"><b style="color: hsl(234, 85%, 45%);">Visual</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <b>72</b> / 100</p>
            </div>
            <button>Continue</button>
        </section>
    </main>
</body>

</html>
```
```css
@import url("https://fonts.googleapis.com/css2?family=Hanken+Grotesk:wght@500;700;800&display=swap");

/* RESET */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/*  */

body{
  overflow: hidden;
}

main {
  display: flex;
  /* justify-content: center;
  align-items: center; */
  text-align: center;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 740px;
  height: 520px;
  font-family: "Hanken Grotesk", sans-serif;
}


/* RESULT CLASS STYLES */

.result {
  width: 380px;
  border-radius: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-image: radial-gradient(hsl(241, 100%, 80%), hsl(241, 100%, 60%));
}

.result-head {
  position: absolute;
  top: 9%;
  font-weight: 500;
  color: whitesmoke;
}

.circle {
  position: absolute;
  top: 20%;
  background-image: linear-gradient(
    hsla(241, 81%, 54%, 1),
    hsla(241, 81%, 54%, 0.9),
    hsla(241, 81%, 54%, 0.8),
    hsla(241, 81%, 54%, 0.7),
    hsla(241, 81%, 54%, 0.6),
    hsla(241, 81%, 54%, 0.5),
    hsla(241, 81%, 54%, 0.4),
    hsla(241, 81%, 54%, 0.3),
    hsla(241, 81%, 54%, 0.2),
    hsla(241, 81%, 54%, 0.1)
  );
  border-radius: 50%;
  width: 200px;
  height: 200px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: whitesmoke;
}

p span {
  font-weight: 800;
  font-size: 65px;
  color: white;
}

.great {
  position: absolute;
  top: 65%;
  font-weight: 800;
  font-size: xx-large;
  color: white;
}

.score {
  position: absolute;
  top: 75%;
  font-size: large;
  padding-left: 4vw;
  padding-right: 4vw;
  color: whitesmoke;
}

/* SUMMARY CLASS STYLES */

.summary {
  width: 370px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.summary h2{
  position: absolute;
  top: 9%;
  left: 55%;
  font-weight: 600;
}

img{
  width: 35px;
  height: 40px;
  padding-left: 1vw;
}

div{
  display: flex;
  border-radius: 15px;
  padding-top: 0.7vh;
}

.reaction{
  position: absolute;
  top: 20%;
  width: 280px;
  height: 55px;
  background-color: hsl(0, 60%, 96%);
}

.power{
  padding-left: 1.5vw;
  padding-top: 1.2vh;
}

.memory{
  position: absolute;
  top: 35%;
  width: 280px;
  height: 55px;
  background-color: hsl(39, 60%, 96%);
}

.verbal{
  position: absolute;
  top: 50%;
  width: 280px;
  height: 55px;
  background-color: hsl(166, 60%, 96%);
}

.visual{
  position: absolute;
  top: 65%;
  width: 280px;
  height: 55px;
  background-color: hsl(234, 60%, 96%);
}

button{
  position: absolute;
  bottom: 6vh;
  width: 280px;
  height: 55px;
  border-radius: 50px;
  background-color: hsl(224, 29%, 35%);
  color: white;
  font-size: 17px;
  font-weight: 600;
}
```
## Author

- Frontend Mentor - [@Moussa-Esbay](https://www.frontendmentor.io/profile/Moussa-Esbay)

