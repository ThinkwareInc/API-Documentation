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
token
: Authenticates API request - <span style="color: red">Required</span>

###### Example

```
https://{baseurl}/ClientAPI/{endpoint}?token={token}
```

Successful authentication will continue with your request.  Any issues authenticating the API token will return an error.
{: .info }

