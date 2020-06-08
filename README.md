# sass-color-shading
My own take on shading colours with Sass making use of a technique commonly used to shade colours in various artistic pieces. I wrote an article explaining the process behind this code: [Improve how you shade colours with Sass (2/2)](http://harryphillips.local/#dynamic-colors-with-sass-part-2)

### ```adjust-shading()```
This is the main, driving function behind the shading. It takes a colour, some parameters, and returns a shaded colour.

### ```dim()``` and ```brighten()```
These are the alternatives to ```darken()``` and ```brighten()```. They can be used similarly but instead of using a percentage you pass in a simple shading "level". The shading level can start from 1 and increase linearly to increase the intensity of the shade.

### ```color2hsv()```
This is a function I wrote to convert an existing Sass colour to HSV, this is because experimentations I did before writing the code involved using HSV colours rather than RGB or HSL.

### ```hsva()```
You can use this function to create a Sass colour using HSV/HSB values. It simply converts your HSV parameters to HSL and returns a colour.
