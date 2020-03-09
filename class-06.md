# Objects

### What is it?

##### Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, vriables and fuctions take on new names.

##### In objects, variables become properties and functions become methods

##### The object represents a hotel. It has five properties and one method. THe object is in curly braces it is stored in the variable hotel.

##### Example: var hotel = { name: 'Quay', rooms: 40, booked: 25, gym: true, roomTypes: ['twin', 'double', 'suite'], checkAvailability: function() { return this.rooms - this.booked; } };

##### THe above object is a hotel and it has properties (name rooms, booked, gym, roomTypes) values (string, number, number, Boolean, array) and a method (checkAvailability)

### Literal Notation

##### easiest and most popular way to create objects

##### var hotel = { name: 'Quay', rooms: 40, booked 24, checkAvailability: function () { return this.rooms - this.booked; } }

### Accessing an objectd and dot notation

##### You access the properties or methods of an object using dot notation. Also by using square brackets.

##### var hotelName = hotel.name; var roomsFree = hotel.checkAvailability();

##### var hotelName = hotel['name'];

### Document Object Model

##### Specifies how browsers should create a model of an HTML page and how JS can access and update the contents of a web page while it is in the browser window.

##### dom tree on page 187 is great example

##### To access and update the dom tree, one must 1.) locate the node that represents the element you want to work with. and 2.) use its text content, child elements, and attributes.

##### To access element:  getElementById(), querySelector()

##### Select multiple elements by:  getElementByClassName (), getElementsByTagName(), querySelectorAll()

##### Traversing between element nodes: parentNode, previousSibling/nextSibling, firstChild/lastChild

### Changing DOM queries

##### methods that find elements in the DOM tree are called DOM queries. When you need to work with an element more than once, you should use a variable to store the result of this query.

##### getElementById('one')';

##### When people talk about storing elements in variables, they are really storing the location of the element(s) within the DOM tree in avariable.

##### Methods that select individual elements: documdent.getElementById('one')

##### 
