---
title: /GetSSOToken
position: 3.0
type: get
description: Get Single Sign On Token
right_code: |
  ~~~ json
  {
    "ssotoken": "2bdcc5208a4e45638f7a647fe69ef4a5467de101b4294ec49ce2cfceb4d15aacb9b530cc220e47c0bbcb976bfcd413028ed0b6c5a252443fa2834ecf26ba4b0d"
  }
  ~~~
  {: title="Response" }

  ~~~ json
  {
    "status":"Error:",
    "message":"Unauthorized"
  }
  ~~~
  {: title="Error" }
---
userid
: The UserID of the user you want to authenticate - <span style="color: red">Required</span>

This endpoint will provide a token that can be used during single sign on to authenticate the user.
{: .info }

###### Example

```
https://{baseurl}/ClientAPI/GetSSOToken?token={token}&userid=exampleid
```

<!-- Lists all the photos you have access to. You can paginate by using the parameters listed above.

~~~ javascript
$.get("http://api.myapp.com/books/", { "token": "YOUR_APP_KEY"}, function(data) {
  alert(data);
});
~~~
{: title="jQuery" }

~~~ python
r = requests.get("http://api.myapp.com/books/", token="YOUR_APP_KEY")
print r.text
~~~
{: title="Python" }

~~~ javascript
var request = require("request");
request("http://api.myapp.com/books?token=YOUR_APP_KEY", function (error, response, body) {
  if (!error && response.statusCode == 200) {
    console.log(body);
  }
});
~~~
{: title="Node.js" }

~~~ bash
curl http://sampleapi.readme.com/orders?key=YOUR_APP_KEY
~~~
{: title="Curl" } -->
