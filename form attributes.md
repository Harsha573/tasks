HTML.FORM ATRIBUTES:-
There are 5 types of attributes.They are

[1]The Action Attribute:

The action attribute defines the action to be performed when the form is submitted.
Usually, the form data is sent to a file on the server when the user clicks on the submit button.

In the example below, the form data is sent to a file called "action_page.php". This file contains a server-side script that handles the form data:

Example:=

On submit, send form data to "action_page.php":

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>

[2]The Target Attribute:-

The target attribute specifies where to display the response that is received after submitting the form.

The target attribute can have one of the following values:

Value	                   Description
_blank      	The response is displayed in a new window or tab
_self	        The response is displayed in the current window
_parent	        The response is displayed in the parent frame
_top	        The response is displayed in the full body of the window
framename	    The response is displayed in a named iframe

The default value is _self which means that the response will open in the current window.

Example
Here, the submitted result will open in a new browser tab:

<form action="/action_page.php" target="_blank">

[3]The Method Attribute:-

The method attribute specifies the HTTP method to be used when submitting the form data.

The form-data can be sent as URL variables (with method="get") or as HTTP post transaction (with method="post").

The default HTTP method when submitting form data is GET. 

Example;-

This example uses the GET method when submitting the form data:

<form action="/action_page.php" method="get">

[4]The Autocomplete Attribute:-

The autocomplete attribute specifies whether a form should have autocomplete on or off.

When autocomplete is on, the browser automatically complete values based on values that the user has entered before.

Example
A form with autocomplete on:

<form action="/action_page.php" autocomplete="on">

[5]The Novalidate Attribute:-

The novalidate attribute is a boolean attribute.

When present, it specifies that the form-data (input) should not be validated when submitted.

Example
A form with a novalidate attribute:

<form action="/action_page.php" novalidate>