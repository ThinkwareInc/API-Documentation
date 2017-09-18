---
title: Authentication
position: 2
---
token
: Authenticates API request - Required

###### Example

```
https://{baseurl}/?token={token}
```

Successful authentication will continue with your request.  Any issues authenticating the API token will return an error.
{: .info }

###### Error

```
{
    "status":"Error:",
    "message":"Unauthorized"
}
```
{: .error }
