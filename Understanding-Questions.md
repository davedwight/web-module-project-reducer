# Understanding Questions:
1. What are the steps of execution from the pressing of the 1 button to the rendering of our updated value? List what part of the code excutes for each step.
* The user presses the 1 button.
* The onClick event listener triggers the handleClick event handler
* The addOne function is called inside the dispatch function.
* The addOne function returns the object: {type: ADD_ONE}
* dispatch sends this value to the reducer
* the switch statement in the reducer goes to the ADD_ONE case where it spreads the state and then changes state.total to the current value plus one
* changing state re-renders the App component which displays the current value of state
...

* TotalDisplay shows the total plus 1.
