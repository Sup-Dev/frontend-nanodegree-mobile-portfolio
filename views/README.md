# Running the application
1. Run pizza.html to run the application.

# Performance optimizations
* Removed render blocking in `updatePositions` function by separating rendering from js execution.
* Fixed render blocking js in `changePizzaSizes` function while changing pizza sizes.
* Used `getElementsByClassName` instead of `querySelectorAll` and `getElementById` instead of `querySelector`.
* Moved `var pizzasDiv = document.getElementById("randomPizzas");` outside the for loop at __line-486__ to avoid multiple DOM calls.
* Moved `document.getElementById("movingPizzas1")` outside the for at __line-565__.
* Number of pizzas are dynamically generated based on the screen height at __line-561__.