# Lab 2 - JQuery

## What is jQuery, and what is it purpose?
JQuery is a third-party library to Javascript, and it is commonly used amongst Javascript programmers. The purpose of the library is facilitate HTML traversals, manipulations, animation, event handling etc. Download the library on the following [page](https://jquery.com/download/) and follow the instructions. An API is provided at their [website](https://api.jquery.com). JQuery also provides an in-depth [learning page](https://learn.jquery.com) with information and tutorials. [Skeleton code](https://github.com/davyie/SDA_WWW_Lab2) is provided for you to work on and you can change what ever you like in the code.

Outline of the assignment is as follows, first few tasks regards traversal. Then manipulation and event handlers are presented together with a few tasks. Afterwards, callback functions are presented together with related tasks. Lastly, to tie everything together we will build form validator.

### Assignment 1 - Traversal
First assignment regards traversal of HTML elements with jQuery. Traversal is the first building block of jQuery, and it is especially important because we want the ability to target correct HTML elements at our fingertips. The assignments of this section regards traversal of html documents. Read the following documents [w3school](https://www.w3schools.com/jquery/jquery_selectors.asp), [jquery](https://learn.jquery.com/about-jquery/how-jquery-works/), [traversing](https://www.w3schools.com/jquery/jquery_traversing.asp) and solve the problems.


1. What is the purpose of \$ in JQuery?
2. Name the three components and their functions of a jQuery statement.
3. Write a statement to get all the paragraph elements.
4. What are the two signs for accessing class and ID elements respectively?
5. Write a statement that gets the first \<div\> element in the document.
6. Write a statement that gets the element with the ID is *slideshow*.
7. Write a statement to get all the elements that belong to the class *story*.
8. Write a statement to target both \<div\> and \<p\> elements.
9. Write a statement to target the element with a link attribute.
10. Write a statement to target the even rows in a table.

### Assignment 2 - Manipulation
Now that you have learnt to target certain elements in a HTML document, it can also be fun to be able to manipulate the elements, e.g. change background color or hide some. In this section you will learn how to add, delete and change elements of a HTML document. Relevant information can be found in the following links, [w3school](https://www.w3schools.com/jquery/jquery_hide_show.asp), [ict](https://www.ict.social/javascript/jquery-basics/replacing-content-cloning-with-jquery-dom).

1. Write a statement that adds a blue border to every \<div\> element in the document.
2. Write a statement that clones the paragraph element with ID *aboutUS* and append \<span\> Hello World \</span\> afterward.
3. Write a statement that when pressing the button dark mode it changes the background color of the whole document to black and all the texts become white.
4. Write a statement that selects every consecutive list element after the list element with id *newFlavor* in the list.
⋅⋅*  Optional: Describe how the stack works in jQuery.
5. Write a statement that adds a class attribute to the first paragraph in the document.
6. Write a statement that filters all even list element and add a purple background color to all the even elements. Use the ice cream flavor list.
7. Write a similar statement but use a function together with *filter*. Tip: read about modulo operator.

### Assignment 3 - Callback functions and event handlers
Previous section introduced the concept of callback functions. The purpose of callback function is to ensure that code runs in-order. Executing code in-order means code is executed line by line. A callback function runs after a certain action is 100\% done processing, e.g. a button is clicked or a field has been set. Callback function is called as a parameter in another function call, either as a function call or lambda function. Further material can be found in the following [link](https://www.tutorialrepublic.com/jquery-tutorial/jquery-callback.php).

1. Write two statements with the same functionality which is to hide the paragraph with ID *aboutBoots* after hovering over it in slow speed and alerts a message the user.
⋅⋅*  First statement should not incorporate callback.
⋅⋅*  Second statement should incorporate callback.
2. Write two statements which combines the three fields into a single string and display it. Tip: Use map().
⋅⋅*  First statement needs to utilize lambda/anonymous functions.
⋅⋅*  Second statement needs to utilize a common function call.

What are event handlers? An event can be described as something happens on a website e.g. mouse hovering, button click etc. JQuery provides methods for performing actions when an event is happening, and it is called Event binding. Most general event binding method is called .on(). It makes use of callback functions as you have previously learnt about. Following resources are provided at [w3school](https://www.w3schools.com/jquery/jquery_ref_events.asp) and [events](https://learn.jquery.com/events/handling-events/).

1. Write a statement which chains two callback functions after each other. The functions are not supposed to be called until the document has finished loading and you have pressed a button called Yellow Background. You will have to write a function call for *Yellow paragraphs*. This function changes the background color to yellow for all paragraph elements. The callback chain functions starts off with waiting until document is finished loading, followed by a button press which triggers another function that changes the background color of all the paragraphs.
⋅⋅*  Write a statement which prompts a message when hovering over the paragraph with ID *aboutUS*.
⋅⋅*  Write a statement which prompts a message once when hovering over the paragraph with ID *story*. In other words, the message should not appear once again when hovering over the paragraph a second time.

### Assignment 5 - Form validator
In most cases jQuery is used to process information before sending a request from server. This is because servers are processing large amount of data parallel. Sending faulty information leads to decreased performance for servers. As a result throughput lowers which means worse experience for the user. Therefore, it is important to make sure the information sent to servers are valid and correct. Thus, we put the responsibility on the website by implementing a validator with Javascript and jQuery, and this is the assignment for this section. No skeleton code is provide for this exercise.

1. Create a form which has first and last name as two fields. Also add a third and fourth field for email address and telephone number. Lastly, create a comment field which the user can enter miscellaneous information.
⋅⋅*  Optional: Apply CSS to make the form look nice in any design you want.
2. Create a script which validates the form.
⋅⋅*  Email: make sure it has the form of abc@def.se. In other words, make sure there is a prefix, suffix and at-sign.
⋅⋅*  First and last name: make sure they are filled in.
⋅⋅*  Telephone number: make sure it is a swedish number and starts with swedish landcode.
      Landcode of sweden is +46.
⋅⋅*  Comment: make sure it is filled in.
3. After the form is filled out, the user presses a button which sends them to next webpage or sends out an alert. For this assignment you can choose whether to display the result of the validation in a pop up window as an alert or webpage. For each of the fields there should be two statements, and you can choose the format you want to display the statements in.
⋅⋅*  First statement should display whether the field was correctly filled or not.
⋅⋅*  Second statement should display comments on the information that was filled in.
      .⋅⋅*  An example would be to first display wrong in red and then comment on what was wrong with the information filled in.
