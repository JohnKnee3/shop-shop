# 22.1.4

Created a utils/actions.js file and a utils/reducers.js file. This is in place to introduce us to the of using the use reducer hook to update the state of the app. As of right now we simply set and and tested the reducers and did the bare bones for the actions. Next up we are going to learn about global state.

# 22.1.5

We built the globalState. It was a ton to take in and nothing is calling it yet but we are currently able to console.log the actual state. I assume next up is getting it running.

# 22.1.6

Here we refactored categoryMenu, productList and Detail to use the GloabalState. Then we took use state out of Home.js

# 22.2.3

Made all the tests for the cart and then added the reducers to make them pass.

# 22.2.4

Created the Cart/index.js and the Cart/style.css and copy pasted in the basics to get this to styled and displayed. Everyting is currently hardcoded. Then we added CartItem/index.js and cpoy pasted that in as well. Finally we went to Home.js and added <Cart/> and went to Detail.js and added <Cart/>

# 22.2.5

We added the shopping cart emoji to the screen and mde it use the TOGGLE_CART reducer we just made. In the global state we added the cart:[] and cartOpen: false. Then we went to Cart/index.js and imported userStoreContext from the GlobalState and the TOGGLE_CART reducer from our actions file. Finally we added the custom useStoreContext hook in our function and made an if statemment if things are false and also made a function that calls the imported TOGGLE_CART reducer. In the JSX we added an onClick to the close button to use this function.
