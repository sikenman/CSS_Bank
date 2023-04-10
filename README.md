# CSS_Bank
My CSS Experiments of 2023 and beyond

----
## Projects
- four-corner.html 
    - displays planets at the four corners of the web page.
    - displays moon at the center of the page.
    - makes use of css variables
    - prevented text selection
    - animation of Earth, coming towards the moon slowly

### Example CSS Code in four-corner.html
```css
:root {
  --transNeg-Mobile: -50%;
  --transPos-Mobile: 50%;

  --opacity1: 0.65;
  --opacity2: 0.80;
}

.moon {
  position: absolute;
  top: 28%;
  left: 30%;
  z-index: -1;  /* send moon to the back position */
}

.earth-rotate {
  animation: mymove 240s infinite;
}

@media only screen and (max-width: 600px) {
  .top-left {
    transform: translate(var(--transNeg-Mobile), var(--transNeg-Mobile));
  }
  .moon {
    position: absolute;
    top: 20%;
    left: 20%;
  }
}
```