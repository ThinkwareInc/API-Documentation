---
title: 'Authentication'


---

All endpoints require an authentication token to be passed for verification.

# Request

Providing a token on each request grants you access to the endpoint you are requesting.

## Parameters
<hr>
### token | Required
```https://{baseurl}/?token={APITOKEN} ```

## Responses

Successful authentication will continue with your request.  Any issues authenticating the API token will return an error.

```{
    "status":"Error:",
    "message":"Unauthorized"
}```


