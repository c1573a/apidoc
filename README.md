# Get Started

> Our API allows you to shorten your links and add metadata dynamically for apps using modern Javascript frameworks such as React or Angular. To get started request an API Key by filling the form at https://app.ogtag.me/developers

## POST 

### Request

Endpoint: https://ogtag.me/API_KEY



```json
{
    image : string , 
    url : string ,
    description : string ,
    title : string
}
```

### Response 

```json
{
    url : string ,
    status : number ,
    status_message : string ,
    hahs : string
}
```
