## Website Performance Optimization portfolio project

### Getting started

#### Running index.html

Open `index.html` in your browser to run it.

### Optimizations in `index.html`
* Compressed __pizzeria__ and __profilepic__ images.
* External javascript is being asynchronous loaded.
* External CSS link has it's media specified to print.
* Inlined `styles.css` properties.

### Running the pizza application
1. Navigate to the `views` folder.
2. Open `pizza.html` in your browser to run the application.

### Performance optimizations in the pizza application
* Removed render blocking in `updatePositions` function by separating rendering from js execution.
* Fixed render blocking js in `changePizzaSizes` function while changing pizza sizes.
* Used `getElementsByClassName` instead of `querySelectorAll` and `getElementById` instead of `querySelector`.
* Moved `var pizzasDiv = document.getElementById("randomPizzas");` outside the for loop at __line-486__ to avoid multiple DOM calls.
* Moved `document.getElementById("movingPizzas1")` outside the for at __line-565__.
* Number of pizzas are dynamically generated based on the screen height at __line-561__.