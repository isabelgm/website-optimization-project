# Website Optimization
How to view this site.
1. To view the portfolio website download all the files to your computer and open index.html in your browser.

2. To view the pizza.html page, download all the files and navigate to views/pizza.html in your browser.

## Optimization to Frames per Second in pizza.html
To optimize the pizza.html I made the following changes:
1. Changed the ChangePizzaSizes function
    * Defined pizzaContainer outside of the for loop so that we only call
    document.querySelectorAll once.
    * Defined new width and dx outside of for loop so they're
    only calculated once.
2. Changed the UpdatePositions function
    * It no longer defines the scrollTop inside the forLoop. This saves us from
    having to call the document.scrollTop every time we go through the loop.
3. Change the number of sliding pizzas that are created
    * Instead of creating 200 pizzas every time you scroll, the number of pizzas
    created is now determined dynamically depending on window size.
