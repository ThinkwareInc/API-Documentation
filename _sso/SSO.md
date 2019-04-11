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
https://{baseurl}/ClientAPI/SSO?token={token}&userid={userid}&ssotoken={ssotoken}
```
Send the required information with your POST request
{: .info }

Upon completion you will be redirected to the user's dashboard.
