# CSS_Randomness
This repo is for me to explore randomness in CSS animations.  
There is currently no ability to create functions in CSS like we can in JavaScript.  

# Purpose and process
Specifically, we are unable to use Math.random() or some similar function to make random transform/translations in the CSS animation.
There are other ways to do this as I have seen examples where a coder was able to choose random
  images of playing cards using only CSS with no JavaScript.  But the "standard response" seems to be
  that this is not possible without JavaScript.
The missing link in the solution is to access the root element from both JavaScript and CSS.

From JS, use "document.documentElement.style." and from CSS create root variables using ":root{ --variableA:value, --variableB:value}". 
Then in your CSS code you access the variables using "var(--variableA)" and you access this same variable from JavaScript
by using document.documentElement.style.setProperty('--variableA','some_property').

# Run the code
I included a sample of my code in this repository for you to view.  I included the CSS and JS all in the same page as the HTML file.
This should make it easier to download and run for yourself.  Open the console to see additional "behind-the-scenes" details.

Note: I recognize that the code can be optimized and the functions written as arrow functions.  My goal was only to figure out how
to use randomness in animations.  I was hoping to do this purely in CSS, but adding JS does give you more granularity and control.
