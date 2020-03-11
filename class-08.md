# Forms

### Things that get info from users are forms, like search boxes

##### Adding text, making choices, and "submit" buttons are examples of forms

##### Forms work by user input (typing a name and pressing submit, for example)

##### The name of each form control is sent to the server along with values

##### The server processes the information using a programming lanugage

##### The server creates a new page to send back to the browser based on info recieved

##### a form may have several form controls, each gathering different info. The server needs to know which piece of inputted data corresponds with which form element. Example: username=Ivy

##### if the form control allows you to choose from a fixed set of answerss like radio buttons, the web page author will add code that gives eah option an automatic value.

### Form Structure

##### "form" is where form controls live (in the HTML)

##### every form element requries an action attribute. its value is the url for the page on the server taht will recieve the info in the form when it is submitted.

##### Forms can be sent using one of two methods: get or post
###### Get methods: the values from the form are added to the end of the URL specified in the action attribute. Best for short forms like search boxes and when you are just retrieving data from the web server (not sending info that shoujld be added to or deletedf from a database)
###### Post methods: the values are sent in what are known as HTTP headers. As a rule of thumb you should use the post method if your form allows users to upload a file, is very long, contains sensitive info, or addits information to/deletes info from a database

##### "input" is used to create several different form controls. The value of the "type" attribute determines what kind of input they create

##### type="text" creates a single-line text input

##### type="name" is when users enter info into a form, the server needs to know which form control each piece of data was entered into. For example, in a login form, the server needs to know what has been entered as teh username and what has been given sa the password.

##### maxlength: you can use this to limit the number of characters a user may enter into the text field. For example, if you as for a year, maxlength is 4

##### "input" is what you use to have commands such as "type=password" happen (its asking for user input)

##### "textarea" is used to create a multi-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and closing tag. Example: "textarea name="comments" cols="20" rows="4""

##### radio buttons are done by "type="radio"". Example <input type="radio" name="genre" value="rock" checked="checked" /> Rock

##### checkbox: example <input type="checkbox" name="service" value="itunes" checked="checked" /> iTunes

##### dropdown lists are done by name, then "option". Example <option value="ipod">iPod</oprion>

##### multiple select box are by "select", size, and multiple. Example <select name="instruments" size="3"
      multiple="multiple">
      <option value="guitar" selected="selected">
      Guitar</option>

### Lists, Tables, and Forms

##### bullet point styles (list-style-type) for unorodered lists you can use none, disc, circle, and square. For ordered lists you can use decimal, decimal-leading-zero, lower-alpha, upper-alpha, lower-roman, and upper-roman

##### Images can be done with list-style-image. This makes the list dot a shape of whatever you want, like a star or a pony lol

##### you can position the marker with list-style-position. you can either have outside (marker sits to the left of block of text) or inside (the marker sits inside the box of text, which is indented. See page 335 for picture

##### Table of Properties. See page 337 for full list. 

### Events

##### Event types: look at page 246.

##### How events trigger in javascript code

##### Event Handling happens in 3 steps: select the element node(s) you want the script to respond to, indicate which event on the selected node(s) will trigger the response, and state the code you want to run when the event occurs.

