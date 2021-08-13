# local storage

What is the Web Storage API?
The Web Storage API is a set of mechanisms that enable browsers to store key-value pairs. It is designed to be much more intuitive than using cookies.

The key-value pairs represent storage objects, which are similar to objects except they remain intact during page loads, and are always strings. You can access these values like an object or using the getItem() method (more on that later).

What is localStorage in JavaScript?
localStorage is a property that allows JavaScript sites and apps to save key-value pairs in a web browser with no expiration date. This means the data stored in the browser will persist even after the browser window is closed.

There are two type of storage : local storage and session storage

 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt() or parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.

 Calling `setItem()` with a named key that already exists will silently overwrite the previous value. Calling `getItem()` with a non-existent key will return null rather than throw an exception.

Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the `getItem() and setItem()` methods, you can simply use square brackets. For example, this snippet of code:

            var foo = localStorage.getItem("bar");
              // ...
             localStorage.setItem("bar", foo);
             could be rewritten to use square bracket syntax instead:

               var foo = localStorage["bar"];
                // ...
                localStorage["bar"] = foo;

There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).

            interface Storage {
                deleter void removeItem(in DOMString key);
                       void clear();
                   };
Calling removeItem() with a non-existent key will do nothing.

How does localStorage work?
To use localStorage in your web applications, there are five methods to choose from:

1. setItem(): Add key and value to localStorage
2. getItem(): This is how you get items from localStorage
3. removeItem(): Remove an item by key from localStorage
4. clear(): Clear all localStorage
5. key(): Passed a number to retrieve the key of a localStorage

setItem(): How to store values in localStorage
Just as the name implies, this method allows you to store values in the localStorage object.

It takes two parameters: a key and a value. The key can be referenced later to fetch the value attached to it.

window.localStorage.setItem('name', 'Obaseki Nosa');
Where name is the key and Obaseki Nosa is the value. Also note that localStorage can only store strings.

To store arrays or objects, you would have to convert them to strings.

To do this, we use the JSON.stringify() method before passing to setItem().

const person = {
    name: "Obaseki Nosa",
    location: "Lagos",
}

window.localStorage.setItem('user', JSON.stringify(person));

getItem(): How to get items from localStorage
To get items from localStorage, use the getItem() method. getItem() allows you to access the data stored in the browser’s localStorage object.

getItem() accepts only one parameter, which is the key, and returns the value as a string.

To retrieve a user key:

window.localStorage.getItem('user');
This returns a string with value as:

“{“name”:”Obaseki Nosa”,”location”:”Lagos”}”
To use this value, you would have to convert it back to an object.

To do this, we make use of the JSON.parse() method, which converts a JSON string into a JavaScript object.

JSON.parse(window.localStorage.getItem('user'));

removeItem(): How to delete localStorage sessions
To delete local storage sessions, use the removeItem() method.

When passed a key name, the removeItem() method removes that key from the storage if it exists. If there is no item associated with the given key, this method will do nothing.

window.localStorage.removeItem('name');
clear(): How to delete all items in localStorage
Use the clear() method to delete all items in localStorage.

This method, when invoked, clears the entire storage of all records for that domain. It does not receive any parameters.

window.localStorage.clear();
key(): How to get the name of a key in localStorage
The key() method comes in handy in situations where you need to loop through keys and allows you to pass a number or index to localStorage to retrieve the name of the key.

var KeyName = window.localStorage.key(index);

localStorage limitations
As easy as it is to use localStorage, it is also easy to misuse it. The following are limitations, and also ways to NOT use localStorage:

1. Do not store sensitive user information in localStorage
2. It is not a substitute for a server based database as information is only stored on the browser
3. localStorage is limited to 5MB across all major browsers
4. localStorage is quite insecure as it has no form of data protection and can be accessed by any code on your web page
5. localStorage is synchronous, meaning each operation called would only execute one after the other
