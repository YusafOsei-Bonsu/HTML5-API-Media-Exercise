# Exercise: Using HTML5 APIs and Media

You have been asked to create a dynamic web site for a car dealership. To start with, the dealership wants to see a prototype/draft web page that has three features:

1. Visitors to the site can view a list of cars that the dealership has available to sell and a button to click to see what the costs of those cars are.
2. Visitors can enter information about their vehicle and make and model and it can be stored in the site and retrieved so that dealership sales representatives can give prospective buyers a quote on their car for a trade in.
3. Visitors can play audio files of previous customer testimonials about their experiences dealing with the dealership.

## Task 1: Use selectors and web storage to handle information

### **Scenario**

For the first two features of the web page prototype, you need to set up the functionality to handle different held on the server and informers to go to the server. You need to:

1. Allow visitors to click to see a change in multiple categories of information on the fly
2. Allow visitors to input information for web storage and preview if what they submitted is correct

You have already set up an HTML5 web page setup with some containers for the information. You need to add code so that your page has the desired functionality.

### **Exercise**

Your assignment for this task is to create code for two related components on the web page prototype:

1. Create an item list that displays the cars in inventory when the page loads and add functionality to match multiple elements (the cars to their respective cost) using selectors from within an HTML5 document. For car cost display, create a selector to find and modify multiple elements or instances of objects. In this case, use the div containers to hold the car models and an interactive button to display their cost. The cost of each car is as follows:
   - Mustang - $50, 000
   - Corvette - $45, 000
   - Porsche - $53, 000
2. Create an area for visitors to enter the model and make of their car. They will need to input and submit their info and can preview what they submitted if desired.

Before you start, open `bestCars_t1.html` to write your code for this task. Most of the HTML code as well as a bit of JavaScript is there for you to begin with. You will need to add most of the JavaScript code within the JavaScript tags and a bit of code in the body of the HTML.

| Step | Instructions | Complete? |
| ---- | ------------ | --------- |
| 1 | Add a button that calls a JavaScript function called "doit", which will run the selector. | |
| 2 | For car cost display, create a selector to find and modify multiple elements or instances of objects. In this case, use the div containers to hold the car models and an interactive button to display their cost. | |
| 3 | Create a counter to count the instances of the div (cars in stock) and put it in an array with a result. | |
| 4 | Create code to return the contents that are stored in the results variable, which add values to the array. | |
| 5 | Make the cost under the car models change to the actual figures. To do this, set up a results output in the JavaScript to change each of the values in the `<div>` that are identified by class=note. | |
| 6 | For the second component, you need to create reference in JavaScript to the HTML interface GUI input and output fields. Start by adding variables for each of the fields (both input and output) and then a function with a reference to each. | |
| 7 | For the buttons that visitors use to submit their car make and model and confirm their information, put code listeners on each of the buttons with respective ids of "store data" and "retrieve data". | |
| 8 | Write the functions for each of the buttons that make use of the web session storage object. Each function should address the session storage object and give it a property name of your choosing. The store data function will put information into the session storage object and the retrieve data function will take information out of it. | |

## Task 2: Add an audio player with controls to web page

### **Scenario**

You already have fulfilled the first two requirements of the web prototype by setting up functionality that allows visitors to view the cost of those cars and enter information about their vehicle and make and model.

Now you need to add functionality so visitors can play audio files of previous customer testimonials about their experiences dealing with the dealership.

### **Exercise**

Your assignment for this task is to add code for an audio player to the dealership web page prototype. You need to set it to auto play. You also need to know the position of the playback head for visitors.

Before you start, open `bestCars_t2.html` to write your code for this task. This file includes all the code needed from Task 1 to start adding the code required for Task 2.

| Step | Instructions | Complete? |
| ---- | ------------ | --------- |
| 1 | Add code in the audio element tags so that the audio auto plays. | |
| 2 | Create an area to put the time of the audio using the current time property. | |
| 3 | Set up an id called aud that can be referred to and initialized to get the playback head position.| |
| 4 | You need to find out where the playback is in the testimonial. Write a JavaScript function to do this. It will need to measure the time in intervals. | |
| 5 | Add a measure function inside the JavaScript and set it up as an id in the audio element so it can be referenced. Then create a global variable to represent that id. | |
| 6 | Initialize the aud variable in the onload function that you created so it gets the aud element. | |