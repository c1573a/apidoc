# Get Started

> Our API allows you to shorten your links and add metadata dynamically for apps using modern Javascript frameworks such as React or Angular. To get started request an API Key by filling the form at https://app.ogtag.me/developers

## POST 

### Request

Endpoint: https://ogtag.me/API_KEY



```js
{
    image : "string" , 
    url : "string" ,
    description : "string" ,
    title : "string"
}
```

Example Request 

```js

let obj = {
    url : "https://app.ogtag.me",
    image : "https://app.ogtag.me/static/media/lightn.21713b21.jpg",
    description : "Shorten your links"
}
fetch("https://ogtag.me/API_KEY" , {
    method : "POST" ,
    body : JSON.stringify(obj) 

})
.then((res) => res.json() )
.then((data) => console.log("🚧 shorten url: " + data.url ))


```

### Response 

```js
{
    url : "string" ,
    status : "number" ,
    status_message : "string" ,
    hash : "string" ,
    type : "string"
}
```
### Default Values
To change the values just specify them to overwrite them.

tag | value |
----|-------|
type|article|
