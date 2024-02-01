# NP HTML5, CSS3, and JavaScript 6e Tutorial 12, Case Problem 1

## Instructions:
1.  Use your editor to open the na_home_txt.html and na_styler_txt.js files from the html12 > case1 folder. Enter your name and the date in the comment section of each file, and save them as na_home.html and na_styler.js respectively.
2.  Go to the na_home.html file in your editor. Go to the document head and add a script element for the na_styler.js file. Load the file asynchronously. Save your changes to the file.
3.  Go to the na_styler.js file in your editor. Add an event listener that runs the setStyles() function when the page loads.
4.  Create the setStyles() function using the commands listed in Steps 5 through 10.
5.  Christine wants one of five fancy style sheets to be randomly used when the page is opened. Declare the styleNum variable equal to the value returned by the randInt() function, using 5 as the parameter value.
6.  Create an element node for the link element and set its rel attribute to "stylesheet", its id attri¬bute to "fancySheet", and its href attribute to "na_style_num.css" where num is the value of the styleNum variable. Append the fancySheet style element to the document head, adding it to the document's style sheets collection.
7.  Christine wants users to be able to choose between the five fancy style sheet themes she has created by clicking thumbnail images from a figure box. Create an element node named figBox for the figure element. Set its id attribute to "styleThumbs" and append it to the div element with the ID "box".
8.  Next, populate the figure box with preview images of the five fancy style sheets. Insert a for loop with an index that goes from 0 up through 4 and each time through the loop do the following:
    a.  Create an img element node named sheetlmg with a src attribute of "na_small_num.png" and an alt attribute value of "na_style_num.css" where num is the value of the index in the for loop.
    b.  Have the browser load a different style sheet when the user clicks one of the thumbnail images by adding an event handler to sheetImg that runs an anonymous function changing the href attribute of the link element with the ID "fancySheet" to the value of the alt attribute of the event target.
    c.  Append sheetImg to the figBox element node.
9.  Next, design the appearance of the thumbnail figure box. Create an embedded style sheet named thumbstyles and append it to the document head.
10.  Add the following style rules to the thumbStyles style sheet: figure#styleThumbs { position: absolute; left: 0px; bottom: 0px; } figure#styleThumbs img { outline: 1px solid black; cursor: pointer; opacity: 0.75; } figure#styleThumbs img:hover { outline: 1px solid red; opacity: 1.0; }
11.  Document your work with informative comments and then save the JavaScript file.
12.  Open the na_home.html file in your browser. Verify that by clicking the thumbnail images in the lower-left corner of the page, the document is displayed in a different style theme. Further verify that reloading the page randomly selects a style theme from one of the five style sheet files.
