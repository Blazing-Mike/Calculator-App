# Frontend Mentor - Calculator app solution

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

### The challenge

Users should be able to:

- See the size of the elements adjust based on their device's screen size
- Perform mathmatical operations like addition, subtraction, multiplication, and division
- Adjust the color theme based on their preference

### Screenshot

![]('\design\desktop-preview.jpg')



### Links

- Solution URL: [Add solution URL here](https://github.com/Blazing-Mike/Calculator-App)
- Live Site URL: [Add live site URL here](http://calulator-app.surge.sh)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Vanilla Javascript

### What I learned

```js
function calculate(event) {
    // current clicked buttons value
    const clickedButtonValue = event.target.value;
  
    if (clickedButtonValue === '=') {
      // check if the display is not empty then only do the calculation
      if (display.value !== '') {
        // calculate and show the answer to display
        display.value = eval(display.value);
      }
    } else if (clickedButtonValue === 'reset') {
      // clear everything on display
      display.value = '';
    } else if (clickedButtonValue == 'del'){
        display.value = display.value.slice(0, -1);
        //removes lastly typed number
    }  else {
      // otherwise concatenate it to the display
      display.value += clickedButtonValue;
    }
  }
```

### Continued development

- Coming up with javascript code to solve a problem in record time( concvert problem statement to code)

### Useful resources

- [Build a javscript calculator](https://www.section.io/engineering-education/building-a-calculator-a-javascript-project-for-beginners/) - This helped me to see how a demo calculator app is built, so i refrenced it when i has issues.

## Author
- Frontend Mentor - [@Blazing Mike](https://www.frontendmentor.io/profile/Blazing-Mike)
- Twitter - [@Omo sathoshi](https://www.twitter.com/Mikeoxygen1)



