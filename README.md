# Frontend Mentor - Calculator app solution

This is a solution to the [Calculator app challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/calculator-app-9lteq5N29). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- See the size of the elements adjust based on their device's screen size
- Perform mathmatical operations like addition, subtraction, multiplication, and division
- Adjust the color theme based on their preference

### Screenshot

![]('\design\desktop-preview.jpg')



### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

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
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/Blazing-Mike)
- Twitter - [@yourusername](https://www.twitter.com/Mikeoxygen1)


