# JavaScript-Control-Structures-solution

Download Here: [JavaScript Control Structures solution](https://jarviscodinghub.com/assignment/javascript-control-structures-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

In this assignment you will revise assignment 1 to include JS control structures to validate user input.

Part I HTML (product_order.html)

1. Revise product_order.html so that each of the form controls has an empty tag associated with it. The can be coded to the right of the control or below the control. The purpose of the span is to serve as a label or output area for error messages. Each will need a unique ID value – use err1 – err10:

…


…

Save the revised changes – product_order.html

Part II – JavaScript (product_order.js)

1. Revise the calcTotal() function so that it includes JavaScript Control Structures to perform user input validation. If the input is incorrect, use the document object’s getElementById() method to display an error message to the span tag associated with the form control (you may use HTML5 input validation if applicable). The output from the previous assignment should not be displayed in the ‘output’ division if any user input errors are detected:

Start by creating a Boolean flag variable that initially assumes all input is correct or valid. Reset the flag variable if an error is found:
var valid = true;
if (isNaN(quantity) || quantity < 1) { document.getElementById("err2").innerHTML = "Quantiry Must Be Numeric and Greater than 0."; valid = false; } The above if statement checks to see if the value of quantity is a number greater than 0 using the isNaN() function and a comparison operator. If the variable is not a number or less than 1, an error message is written to the span tag associated with the loanAmount control and the flag variable is reset to false. The following validation checks should be performed:  Product – cannot be empty  Quantity – must be numeric and greater than 0  Unit Price – must be numeric and greater than 0  Discount Rate – must be numeric and greater than 0  Date – cannot be empty and length must be between 8 and 10.  First Name – cannot be empty and length must be greater than 1  Last Name – cannot be empty and length must be greater than 1  Payment Type – cannot be empty  Card Number – must be a 16 digit integer number  Security code – must be a 3 digit number The output should only be displayed if all input is correct (the following is pseudo-code, use correct syntax): If (valid) { document.getElementById("output").innerHTML = Thank you, first_name last_name. Your order total is order_total. } Be sure to comment your code. Save this page as product_order.js
