# Assignment 3: Dynamic Front-end Web Application

## Briefing

![Image: Screenshot of Weather App by Vanilla JS Academy](/assets/assignment-03__header.png)
[Image: Screenshot of Weather App by Vanilla JS Academy](https://vanillajsacademy.com/projects/weather/)

This week, the assignment is to created a dynamic front end web application. This means that it must:
  * Connect with an API (e.g. weather, time)
  * Include an interactive element that responds to an event (e.g. click, scroll, mouseover, etc.)
  * Be responsive to the screen size

There are MANY APIs out there. Here's a list you might consider exploring: [list of public apis](https://github.com/public-apis/public-apis) If the API is marked **CORS: No**, or **Auth: OAuth**, you won't be able to use it for this assignment.

## Required Readings
* [Elements of UI Engineering](https://overreacted.io/the-elements-of-ui-engineering/)
* [How to Connect to an API with JavaScript](https://www.taniarascia.com/how-to-connect-to-an-api-with-javascript/)
* [Reactive UIs in Vanilla JS](https://css-tricks.com/reactive-uis-vanillajs-part-1-pure-functional-style/)

## Example Projects
Note that these are not finished, polished apps, just a jumping off point.
* [Weather App](https://github.com/muji786/weather-app)
* [Music Genres + Feelings](https://github.com/muji786/spring2024-dynamic-web-development/a3-cat-frontend-web-app)

## Requirements

### Part 1: Sketching, Wireframes, and Design specifications
This is another opportunity to practice design, as well as making a making a plan *before* you start coding. Please include:

* 1. Annotated hand-drawn sketches of your layout and content. Because this week there are more dynamic elements, be sure to include different **states** of your app.
* 2. Wireframes that translate your hand-drawn sketches into a digital format
* 3. A "final" design that breathes life into your wireframes
* 4. Basic style guide that is specifies at the very least about your typographic hierarchy, your grid, and color palette and acts as your project's visual design source during development. 

### Part 2: Development
This is another chance to practice translating your designs into code, in the same way was the last assignment. This time, you'll enhance what you did last week with more complex JS. You will 
* 1. Create an HTML structure that best uses semantic HTML to structure your content
* 2. Define CSS rules that follow as best as possible BEM conventions that structure your layout and style your DOM elements
  * you must use BEM conventions to apply CSS classes
  * uses percentage widths/flexbox/media queries to create a responsive layout
* 3. Write JavaScript that:
  * Uses `fetch()` to load data from an API
  * Uses API data to dynamically change the DOM
  * Is organized in the style of functional Reactive UI (see [Reactive UIs in Vanilla JS](https://css-tricks.com/reactive-uis-vanillajs-part-1-pure-functional-style/) as a guide)
  * Contains at least one interactive element that responds to an event (mouseover, scroll, click, etc.)


### Part 3: Deployment
Your website will be served using a static web server on **Glitch** and will be pulled from a remote Github repository. You will need to practice good git tracking and connect your local git repository to a remote Github Repository. 

You can copy the code from Assignment `02` from last week and put your static HTML, CSS, and JavaScript files into the correct directories.

**e.g.**:
* `index.html`
* `/views`:
  * `about.html`
* `/public`:
  * `/js`:
    * `main.js`
  * `/css`:
    * `main.css`

### Part 4: Documentation
* You must have a README.md that explains:
    * how to set up and run your application.
    * how you built your HTML page
    * inspiration, process documentation, struggles, references, and questions, like your ITP blog
    * and how you deployed your work to [Glitch.com](https://glitch.com).
  * You may use this [README template](/templates/readme-template.md) to structure your README documentation and blog post
