# Running the application
1. Run pizza.html to run the application.

# Performance optimizations
* Removed render blocking in `updatePositions` function by separating rendering from js execution.
* Fixed render blocking js in `changePizzaSizes` function while changing pizza sizes.
* Used `getElementsByClassName` instead of `querySelectorAll` and `getElementById` instead of `querySelector`.
