# Local Storage for Web Apps

### Persistent local storage is where native client apps have an advantage over web apps

##### The operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.

##### Values may be stored in the registry, INI files, XML files, or some other place according to platform convention.

##### Cookies can be used for persistent local storage of small amounts of data, but have drawbacks, including: 
###### Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
###### Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
###### Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

##### HTML5 fixes these issues, thankfully

##### userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.

##### trusted domains can store 10 times that

### HTML5 Storage

##### It's a way for web pages to store named key/value pairs locally, within the client web browser.

##### Data persists even after you leave the page.

##### It's implemented natively in web browsers, so it is available even when third-party browser plugins are not.

### Check for HTML5 Storage

#####   function supports_html5_storage() {
#####   try {
#####     return 'localStorage' in window && window['localStorage'] !== null;
#####   } catch (e) {
#####     return false;
#####   }
##### }

##### you can also use modernizr:

#####  if (Modernizr.localstorage) {
#####// window.localStorage is available!
##### } else {
#####   // no native support for HTML5 storage :(
#####   // maybe try dojox.storage or a third-party solution
##### }

### Using HTML5 Storage

##### HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

##### interface Storage {
#####   getter any getItem(in DOMString key);
#####   setter creator void setItem(in DOMString key, in any data);
##### };
##### Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-##### existent key will return null rather than throw an exception.

##### Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the getItem() and ##### setItem() methods, you can simply use square brackets. For example, this snippet of code:

##### var foo = localStorage.getItem("bar");
##### // ...
##### localStorage.setItem("bar", foo);
##### …could be rewritten to use square bracket syntax instead:

##### var foo = localStorage["bar"];
##### // ...
##### localStorage["bar"] = foo;

##### The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.
