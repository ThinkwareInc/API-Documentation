---
title: /GetEmployee
position: 1.1
type: get
description: Get Employee Information
right_code: |
  ~~~ json
  [
    {
      "FirstName": "Todd",
      "MiddleName": "",
      "LastName": "Washington",
      "BirthDate": "3/18/1978",
      "HomePhone": "5555555555",
      "HomeEmailAddress": "",
      "WorkPhone": "2222222222",
      "WorkEmailAddress": "xxxxxx@thinkwareinc.com",
      "Gender": "Male",
      "MaritalStatus": "",
      "Status": "Active",
      "AddressLine1": "1024 Birch Ave",
      "AddressLine2": "",
      "AddressLine3": "",
      "City": "Atlanta",
      "State": "GA",
      "ZipCode": "28741",
      "Division": "division (0001DIVISION)",
      "Department": "Sales (001SLS)",
      "Location": "",
      "Shift": "1",
      "Job": "Sales (SALES)",
      "Project": "N/A",
      "BenefitGroup": "N/A",
      "PayGroup": "N/A",
      "StandardHours": "",
      "EmployeeType": "Full Time Regular",
      "OriginalHireDate": "11/1/2015",
      "EmploymentHistory": null,
      "PTO": null,
      "DirectDepositItems": null
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
: The Company ID of the employee - Required

clientid
: The Client ID of the employee - Required

employeeid
: The Employee ID of the employee - Required

This Endpoint includes EmploymentHistory, PTO, and DirectDepositItems
{: .info }

###### Example

```
https://{baseurl}/ClientAPI/GetEmployee?token={token}&companyid=1&clientid=001&employeeid=010010001
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
