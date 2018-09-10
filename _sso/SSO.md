---
title: /SSO
position: 3.1
type: post
description: Single Sign On
right_code: |
  ~~~ json
  {
    "status":"Error:",
    "message":"Invalid Token."
  }
  or
  {
    "status":"Error:",
    "message":"User does not exist."
  }
  ~~~
  {: title="Error" }
---
token
: The API key used for authentication - <span style="color: red">Required</span>

UserID
: The UserID of the user you want to authenticate - <span style="color: red">Required</span>

SSOToken
: The token supplied by the /GetSSOToken endpoint - <span style="color: red">Required</span>

This endpoint will provide single sign on into Darwinet 2.0.
{: .info }

###### Example

```
https://{baseurl}/ClientAPI/SSO?token={token}
```
Send the required information with your POST request
{: .info }
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
