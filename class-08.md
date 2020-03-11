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

##### 

