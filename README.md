# JS-Chapter3
JavaScript Chapter 3 Programming Assignment

In this project you create an application that calculates the total cost of items selected from a lunch menu using a for loop and an if statement as part of the program code. The cost of each menu item is stored in the value attribute of an input control on a web form. Because attribute values are treated as text strings, you will have to convert the attribute value to a number using the following JavaScript function:

Number(object.value)

where object is a reference to an input box within the web page. Your application will automatically update the total order cost whenever the user clicks a menu item checkbox. Figure 3-18 shows a preview of the completed project.

![image](https://github.com/user-attachments/assets/4365f02a-0c0c-4275-89cb-50a20f1b2eec)

image Figure 3-18

Do the following:

Use your code editor to open the index.html and script.js files. Enter your name and the date in the comment section of each file and then commit.

Go to the index.html file in your code editor and in the head section add a script element to load the script.js file. Include the defer attribute to defer loading the file until the entire page is loaded. Study the contents of the HTML file, noting that all checkboxes for the menu items belong to the menuItems class. Save your changes to the file.

Go to the script.js file in your code editor. Below the initial comment section, declare a variable named menuItems containing the collection of HTML elements belonging to the menuItem class using the getElementsByClassName() method.

Create a for loop that loops through the contents of the menuItems collection with a counter variable that starts with an initial value of 0 up to a value less than the length of the menuItems collection. Increase the counter by 1 with each iteration. Within the for loop, add an event listener to the menuItems[i] element in the collection (where i is the value of the counter), running the calcTotal() function when that item is clicked.

Create the calcTotal() function to calculate the total cost of the customer order given the selected menu items. Add the following commands to the function:

Declare the orderTotal variable, setting its initial value to 0.

Create a for loop that loops through the contents of the menuItems collection. For menuItems[i] (where i is the counter), apply an if statement that tests whether the item has been checked. If true, increase the value of the orderTotal variable by the value of menuItems[i]. (Hint: Use the Number() function to convert the value of menuItems[i] to a number.)

After the for loop, insert a command to change the innerHTML property of the element with the id "billTotal" to the value returned by the formatCurrency() function using orderTotal as the parameter value.

Commit your changes to the file and then open index+.html in your browser. Verify that the total cost of the order is automatically updated as you select and deselect menu items in the web form.
