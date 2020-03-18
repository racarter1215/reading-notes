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

##### function supports_html5_storage() {
#####  try {
#####    return 'localStorage' in window && window['localStorage'] !== null;
#####  } catch (e) {
#####   return false;
#####  }
#####}
