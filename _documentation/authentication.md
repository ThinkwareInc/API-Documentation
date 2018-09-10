---
title: Authentication
position: 2
right_code: |
  ~~~ json
  {
    "status":"Error:",
    "message":"Unauthorized"
  }
  ~~~
  {: title="Error" }
---
Your API token is available for System level users at the following url:

```
https://{baseurl}/APIToken
```

or by clicking API Token under the gears in the top right.

API Tokens are like passwords..DO NOT share them.
{: .warning }

token 
: Authenticates API request - <span style="color: red">Required</span>

###### This is the API key you will use to authenticate each request.

###### Example

```
https://{baseurl}/ClientAPI/{endpoint}?token={token}
```

Successful authentication will continue with your request.  Any issues authenticating the API token will return an error.
{: .info }

