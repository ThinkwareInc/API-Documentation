---
title: /GetClientCodes
position: 1.0
type: get
description: Get Client Codes
right_code: |
  ~~~ json
  [
    {
      "CodeID": "001ADM",
      "CodeDescription": "administration"
    }, {
      "CodeID": "001SLS",
      "CodeDescription": "Sales"
    }
  ]
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
companyid
: The Company ID of the employee - <span style="color: red">Required</span>

clientid
: The Client ID of the employee - <span style="color: red">Required</span>

type
: Code Type: <br/> Departments, Divisions, EmployeeTypes, Jobs, Locations, Shifts, Statuses, Paycodes - <span style="color: red">Required</span>

This Endpoint returns client code information
{: .info }

###### Example

```
https://{baseurl}/ClientAPI/GetClientCodes?token={token}&companyid=1&clientid=001&type=Departments
```
