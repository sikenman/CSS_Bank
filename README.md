# CSS_Bank
My CSS experiments of 2023 and beyond

----
## Projects
- four-corner.html 
    - displays planets at the four corners of the web page.
    - displays moon at the center of the page.
    - makes use of css variables

### Example CSS Code in four-corner.html
```css
.moon {
  position: absolute;
  top: 28%;
  left: 30%;
  z-index: -1;  /* send moon to the back position */
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