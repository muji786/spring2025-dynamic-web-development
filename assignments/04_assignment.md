# Assignment 4: API Love You - Oh CRUD

## BRIEFING

This week your assignment is to **leap into the world of server-side programming** with Node.js/Express.js. In this project, you will write server-side JavaScript to **create an API** that accepts AJAX request coming from a client-side web application (that you've built) to **create**, **read**, **update**, and **delete** data that are living on your server. 

## READINGS
* [Back-end Foundations Guide](../guides/backend-foundations-guide.md)

* [What is Node.js](https://www.youtube.com/watch?v=RF5_MPSNAtU&t=5s)
* [Building and API in Node.js Series - Coding Train](https://www.youtube.com/watch?v=P-Upi9TMrBk&list=PLRqwX-V7Uu6Yyn-fBtGHfN0_xCtBwUkBp)

## ADDITIONAL REFERENCES
* [Data & APIs Coding Train Series by @shiffman](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6YxDKpFzf_2D84p0cyk4T7X)
* [Simple Express API Tutorial by @joeyklee](https://github.com/joeyklee/simple-express-api)
* [Express Tutorial - Flavio Copes](https://flaviocopes.com/express/)
  
## REQUIREMENTS

### PART 1: DESIGNING YOUR API
* Similar to the previous weeks' assignments, you will start by designing your API on paper. You will be required to conceptually diagram how your requests and data will flow between your client and server. 

### PART 2: DEVELOPMENT
* **Server Side**:
  * You will need to use `npm init` to create your Node project
  * You will add dependencies using `npm install`
  * Your server-side code will use Express.js to define meaningful API routes that allow you to CREATE, READ, UPDATE, and DELETE data on the server using http requests. You will use:
    * GET: `app.get()`
    * POST: `app.post()`
    * PUT: `app.put()`
    * DELETE: `app.delete()`
  * You will create multiple endpoints that do at least one of the following:
    * Access an API that can't be used client-side, due to CORS or Authentication reasons
    * You will read and write to a JSON file data store
  * Your client side code will be served through your web server by:
    * 1. creating a static file server middleware
    * 2. setting the default API route of your server to send the `index.html` file in your static file directory.
  * You will add the keyword `start` followed by the command to run your server.js file to the "script" property of your `package.json` so you can start your server by running `npm start` (otherwise it won't work with Glitch!). In `package.json`:
  ```json
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "node server.js"
  },
  ```
* **Client Side**:
  * You will use the `async/await` and the `fetch()` function to make network requests that allow your client to communicate with your server's API.
  * The data from the API will be transformed dynamically, using JS, into HTML
  * The focus this week is on creating an API and connected it to the browser, so the design and layout can be simple.
  * Your client side code (HTML, CSS, JavaScript) will be served through your `express` web server.
  * This static server will also serve any necessary CSS and image/video/etc. files

  This is how your code should be structured:
  ```
  yourProject/
    package.json
    package-lock.json
    .gitignore
    index.js
    db/
      data.json
    server/
      your-custom-js-script.js
    public/
      js/
        main.js
      css/
        main.css
      assets/
        mycat.png
  ```


### PART 3: DEPLOYMENT
Your website will be served using **Glitch** and will be pulled from a remote Github repository. You will need to practice good git tracking and connect your local git repository to a remote Github Repository. 

You must ensure that your `package.json` has all of the necessary components in order for your application to run. It should look something like this (but not exactly) -- pay particular attention to the "scripts" section:

```json
{
  "name": "first-api",
  "version": "0.0.1",
  "description": "My first API",
  "main": "server.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "node server.js"
  },
  "author": "Cassie Tarakajian",
  "license": "ISC",
  "dependencies": {
    "express": "^4.17.1"
  }
}
```

If you are using an API and need to store secret keys, you will need to create a `.env` file in your Glitch project, **after** you import it from GitHub, since it won't be checked into your project because of your `.gitignore`. You can access variables in your `.env` file in any Node scripts in `process.env.VARIABLR_NAME`. [See this guide from Glitch for more](https://glitch.com/help/env/).

### PART 4: API DOCUMENTATION
* You must have a file in your repository called `API.md` that contains a list of all endpoints, with the following information:
  * The route, i.e. `/toppings`
  * The HTTP verb, i.e. `GET`
  * Query string parameters, i.e. `q=pepperoni`
  * Any URL parameters, i.e. `/toppings/:name`
  * Request body format, i.e.
  ```json
  {
    topping: "pepperoni"
  }
  ```
  * Response format, i.e.
  ```json
  { 
    description: "A list of pizza toppings.",
    pizzaToppings: [
      "pepperoni",
      "ham",
      "pineapple",
      ...
    ]
  }
  ```
  
### PART 5: README DOCUMENTATION
* You must have a `README.md` that explains:
    * how to set up and run your application.
    * how you built your HTML page
    * inspiration, process documentation, struggles, references, and questions, like your ITP blog
    * and how you deployed your work to [Glitch.com](https://glitch.com).
  * You may use this [README template](/templates/readme-template.md) to structure your README documentation and blog post
