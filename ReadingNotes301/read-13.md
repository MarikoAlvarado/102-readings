# [Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data)

**Client/Server Architecture**

1. Client sends request to server using HTTP protocol
2. Server responds using HTTP protocol

**How The Client Side Sends Data**

- ``action`` attribute form defines where the data will be sent
- The **value** of that action must be either a **relative** *or* **absolute** **URL**

ex/Absolute URL:

```md
  <form action="https://example.com">
```
ex/Relative ULR

```md
<form action="/somewhere_else">
```

**if no value is given to action attr, the data will be sent to the same page that the form is on**

- ``name=value`` of form are sent to server joined with **ampersands(&)**
- server will receive data from client and load a new URL that was defined by the **action attribute**

### GET Method

Browser uses the **GET** method to send a **request** to the server asking for a sources. the **body** of information sent to the server is **appended to the URL** in a **series** of **name=value** pairs, each separated by an **&**

### POST Method

Browser uses the **POST** to ask for a **response** correlating with data that is *already* within the body of the HTTP request if a **form** is used.

#### View HTTP Request Using Dev Tool

1. Open dev tool
2. "Network"
3. "All"
4. Select "___.com" in "Name" tab
5. "Headers"

**if you need to send sensitive data, ~~do not use GET~~ method!**

**if you need to send large amount of data, *use POST* METHOD**

### Receiving Data On the Server

The server receives a **string** and will be **parsed** to get the data as list of **key=value** pairs. Refer to [Express For Receiving Data](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs)

### Sending Files

Files are **binary data**

To **send files**:

1. Use **POST** method
2. Set **value** of **encypt** = ``multipart/form-data``
3. Include 1/+ ``<input type="file">`` so user can select files to upload.

ex:

```md
<form method="post" action="https://www.foo.com" enctype="multipart/form-data">
  <div>
    <label for="file">Choose a file</label>
    <input type="file" id="file" name="myFile">
  </div>
  <div>
    <button>Send the file</button>
  </div>
</form>
```

### Security issues

- Always consider security when sending data to a server
- HTML form are **most common server attack vectors** (where attacks go down)
- How the server handles the data is what can make the data *vulnerable*

1. Be weary of using **character sequences tht look like *executable* code**
2. **Limit** incoming amount of data. Only get what is necessary
3. Store data on a **different** server and only permit access through a different **subdomain/domain**

## Resources

### [Form in HTML5](https://htmlreference.io/forms/)
### [Videos: Styling HTML Forms](https://www.youtube.com/playlist?list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK)
