# automated-a11y-sass

Sass functions that support accessible color contrast ratios

## Requirements

Minimum [dart sass](https://github.com/sass/dart-sass) version 1.33.0.

## Acknowledgments

+ Adapted to use updated WCAG 2.1 contrast calculations and the built in dart-sass 
  `math.pow()` and `math.div()` functions from
  [J. Hogue](https://github.com/jhogue/automated-a11y-sass)
+ Previous ideas used lots of math to replicate a `pow()` function but it was not 
  performant. Then I used a lookup table and that worked pretty well. Better still, 
  [Merovex](https://github.com/Merovex) provided a succinct and performant `pow()` from
  [Hail2u](https://gist.github.com/hail2u/1964056)
+ Luminance function adapted from 
  [Sérgio Gomes](https://medium.com/dev-channel/using-sass-to-automatically-pick-text-colors-4ba7645d2796)
  who borrowed code from [voxpelli](https://gist.github.com/voxpelli/6304812)
+ “Light or Dark?” function also adapted from Sérgio Gomes
+ Contrast ratio calculation adapted from Lea Verou’s 
  [Color.js](https://github.com/LeaVerou/contrast-ratio/blob/gh-pages/color.js)
+ Debugging the `@while` Sass statement help from [Merovex](https://github.com/Merovex)
+ And finally, lots of other various sources of math and approaches to this until I came 
  across the best way to do things (so far)
