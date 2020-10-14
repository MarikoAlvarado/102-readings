### [HOME](README.md)

# [“The Past, Present, and Future of Local Storage for Web Applications”](http://diveinto.html5doctor.com/storage.html)

Cookies were developed for the purpose of storing small amounts of data locally but they have downsides such as:

- they slow down web applications by transmitting the same data repetitively
- they send unencrypted data around the WWW
- the are limited in how much data they can hold (about 4KB)

What's more ideal?

- more storage space
- on the client
- doesn't get wiped out when a page is refreshed
- doesn't get sent to the server

## HTML Storage

Also known as "web storage" or some browser vendors call it **local storage** or **DOM** allows for more storage of key/value pairs locally within the browser. This data is not transmitted to a remote web server. 

Browser that support Local Storage:

- IE 8+
- Firefox 3.5+
- Safari 4+
- Chrome 4+
- Opera 10.5 +
- IPhone 2+
- Android 2+

## Using Local Storage

Local storage pulls the data stored on a key from a key/value pair. The key is a string and data can be strings, booleans, integers, or float since they are supported by JS. **use parseInt() of parseFloat()** to convert the *string*!!

To call an item, either use **[]**, **getItem()** or **setItem()**
To remove item us **removeItem()**

**calling or removing what doesn't exist will result in *null***

## Tracking Changes To Local Storage

Storage events are supportes wherever the *object** being called, removed or cleared is supported. So it is not applicable across all browser versions.

### Storage Event Objects

| Property | String | Description                                                       |
|----------|--------|-------------------------------------------------------------------|
| key      | string | named key that was added removed, or modified                     |
| oldValue | any    | previous value (now overwritten), or null if a new item was added |
| newValue | any    | new value, or null if an item was removed                         |
| url*     | string | the page which called a method that triggered this change         |

## Limitations in Current Browsers

When storing large amounts of integers, floats by strings they tend to take up a lot of data, so expect a ``QUOTA_EXCEEDED_ERR`` to pop up. 



refer to [HTML STORAGE IN ACTION]{http://diveinto.html5doctor.com/storage.html} for example involving a game.

### [HOME](README.md)