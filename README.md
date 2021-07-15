# [Natours: Float Layout with Advanced Responsive Design](https://jacobgrisham.github.io/Float-Layout-with-Advanced-Responsive-Design/)
### Coding project from the Udemy Course [Advanced CSS and Sass: Flexbox, Grid, Animations, and more](https://www.udemy.com/course/advanced-css-and-sass/)
I wrote the code in the sass directory and package.json. The other files were provided by the instructor.

App Demo
![AppDemo](img/appdemo.gif)

Advanced Responsive Design
![ResponsiveDemo](img/respdemo.gif)

## 💡Lessons Learned
- CSS architecture with Sass
- animations
- custom grid with float
- clearfix
- pure css modal/popup
- Sass mixins
- Sass variables
- BEM notation
- responsive images in HTML and CSS
- media queries
- setting up build process with npm scripts

## 🚀 Getting Started
To run this project locally:
- In your terminal, navigate to the root folder and run the following commands
```
$ npm install
$ npm start
```

## 📝 Lecture Notes
[Pseudoclasses](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)
- `:hover`. Trigger by a user mousing over
- `:focus`. Trigger when an element receives focus, such as when using the tab key or when an input is selected with the mouse. Really only applies to inputs, text areas, and buttons.
- `:active`. Trigger when the user presses down the primary mouse button
- A tag, class, or id goes before the :pseudoclass. (i.e. `h1:hover`)

[Transform](https://developer.mozilla.org/en-US/docs/Web/CSS/transform): Selector that lets you move, rotate, warp, and scale elements. Here are a few of the most common:
- `Translate()`. Property that allows you to move an element along the X and Y axis
- `Scale()`. Property that allows you increase or decrease the size of the element from the origin. The origin is the center of the element
- `Rotate()`. Property that allows you to rotate an element.
- If you want multiple transform properties, then write them inside the same selector (i.e `transform: scale(2) rotate (180deg);`)
- [Transform-origin](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-origin): Selector that allows you to change the origin of an element.

Vendor Prefixes: different browsers handle these differently
- Use an [auto-prefixer](https://autoprefixer.github.io/) or the npm package

[Transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/transition): Selectors that set the target and set the timing of changes
- Transition-property. Targets specific properties that you want to apply the transition to. You can target multiple properties (i.e. `transition-property: background, border-radius;`)
- `Transition-duration`. Sets the time it takes to complete the transition. You can target multiple properties (i.e. `transition-duration: 5s, 1s`)
- `Transition-delay`. Sets the time it takes before applying the transitions
- Transition-timing-function. Sets the acceleration curve for the transition. Property values include `ease-in`, `ease-out`, `linear`, and `cubic-bezier(#,#,#,#)`
- Shorthand selector. `Transition: property, duration, timing-function, delay;`
- What __can__ be transitioned? Here's a [list](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties)
- What __should__ be transitioned? While you can transition a lot of things, it may affect the performance of the website. These are the 4 properties that are [recommended](https://www.html5rocks.com/en/tutorials/speed/high-performance-animations/) for animation if you’re concerned about performance. You would be concerned about performance if you’re using 100+ animations on a single webpage, if you work for a big company, or if you tailor to mobile
  1. `translate`
  2. `opacity`
  3. `scale`
  4. `rotate`

[CSS Keyframe Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes)
- `animation-name`
- `animation-duration`
- `animation-timing-function`
- `animation-delay`
- `animation-iteration-count`. How many times should it repeat. Commonly used property value is: `infinite`
- `animation-direction`. Property values include: `forward`, `reverse`, and `alternate`. `Reverse` is useful for making an existing animation go in the opposite direction so that you don’t have to write a new one. `Alternate` is useful for making the animation go forwards __and__ reverse.
- `animation-fill-mode`. Property values include: `forward`, `backwards`, `both`, `none`.  Specifies how an animation should apply styles before and after the animation. `Forward` is useful for persisting the end state of the animation (i.e. after changing color to red upon hover, it will stay red). 
- `animation-play-state`. Property values include: `paused` and `running`. Most often used in Javascript where this property is manipulated.
- Shorthand for declaring property values for animation property: `animation: name, duration, timing, delay, iteration-count, direction, fill-mode, play-state`.

## 📣 Reference
- Section 2: Natours Project - Setup and First Steps, Section 5: Natours Project - Using Advanced CSS and Sass, and Section 6: Natours Project - Advanced Responsive Design of the Udemy Course [Advanced CSS and Sass: Flexbox, Grid, Animations, and more](https://www.udemy.com/course/advanced-css-and-sass/)
