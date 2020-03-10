# Tables

### Tables represent info in a grid format, such as finance reports, schedules, and sports results

##### grids allow us to understand complex data by referencing info on two axes. Each block in the grid is reffered to as a table cell. In HTML tables are written out row by row

##### structure includes "table" which creates a table, "tr" which stands for table row and is under "table", "td" which stands for table data (basically "li" but in a table).

##### "th" is table heading and is used to be the heading for the colunm or row

##### spanning columns is done by td colspan="the number of columns it spans"

##### spanning rows is done by td rowspan="the number of rows it spans"

### Long tables

##### "thead" is where the headings of the table should sit within the element. Example "table, thead, tr, th-date-/th, /tr, /thead/

##### the "tbody" is where the table body will sit in (just like body in basic HTML)

##### "tfoot" is where the footer is in a table, like its HTML counterpart.

##### old code that we can use includes width, spacing, border, and background. You put all of these in the "table" tag at the very beginning of the table.

### Constructor Notation

##### the NEW keyword and the object consturctor create a blank object. You can then add properties and methods to the object.

##### First you create a new object using a combo of the new keyword and the Object() constructor function.

##### Example: var hotel = new Object();
##### hotel.name = 'Quay';
##### hotel.rooms = 40;
##### hotel.booked = 25'
##### hotel.checkAvailability = function() {
#####  return this.rooms - this.booked:
##### };

##### Updating object properties, you use dot notation or square brackets. Example: hotel.name = 'Park'; or hotel['name'] = 'Park';

##### You can delete a property by writing something like delete hotel.name;

##### Sometimes you will want several objects to represent similar things. Object consturctors can use a function as a template for creating objects. First create the template with the object's properties and methods.

##### example: function Hotel(name, rooms, booked) {
##### this.name = name;
##### this.rooms = rooms;
##### this.booked = booked;
##### this.checkAvailability = function () {
#####   return this.rooms - this.booked;
##### };

##### the "THIS" keyword is used instead of the objectd name to indicate that the property or method belongs to the object that THIS function creates.

##### Constructors start with uppercase letter to help you sort them out from other objects.

##### You can create instances of the object using the constructor function. The new keyword followed by a call to the function creates a new object. The properties of each object are given as arguments to the function.

##### Example: var quayHotel = new Hotel('Quay', 40, 25);
##### Example: var partkHotel = new Hotel('Park', 120, 77);

### It is a keyword

##### example: function windowSize() {
##### var width = this.innerWidth;
##### var height = this.innerHeight;
##### return [height, width];
##### };

##### "this" can also call global variables!!!!

### Built in objects

##### Browswer Object Model

##### Document Object Model

##### Global Javascript Objects


