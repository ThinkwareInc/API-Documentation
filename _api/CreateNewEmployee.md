---
title: /CreateNewEmployee
position: 1.2
type: post
description: Create a new Darwinet Employee
right_code: |
  ~~~ json
  [
    {
        "employeeid": "010020115"
    }
  ]
  ~~~
  {: title="Response" }

  ~~~ json
  {
    "status":"Error:",
    "message":"An error has occured."
  }
  ~~~
  {: title="Error" }
---
companyid
: The Company ID of the employee - <span style="color: red">Required</span>

clientid
: The Client ID of the employee - <span style="color: red">Required</span>

employeeid
: The Employee ID of the employee - <span style="color: red">Required</span>

Required Fields listed below should be submitted during your POST request
{: .info }

FirstName
: The First Name of the employee - <span style="color: red">Required</span>

LastName
: The Last Name of the employee - <span style="color: red">Required</span>

SSN
: The Social Security of the employee - <span style="color: red">Required</span>

EEStatus
: The Status of the employee - <span style="color: red">Required</span>

Department
: The Department of the employee - <span style="color: red">Required</span>

Position
: The Position of the employee - <span style="color: red">Required</span>

WorkHoursPerYear
: The Work Hours per year of the employee - <span style="color: red">Required</span>

WorkState
: The WorkState of the employee <br/> ex: OH<br/> - <span style="color: red">Required</span>

DOB
: The Date of Birth of the employee - <span style="color: red">Required</span>

EEClass
: The Employee Class of the employee - <span style="color: red">Required</span>

Email
: The Email of the employee - <span style="color: red">Required - if using on boarding</span>

Gender
: The Gender of the employee

Ethnicity
: The Ethnicity of the employee

PayPeriod
: The Pay Period of the employee

DueDate
: The Onboarding due date

Fields listed below are <span style="color: red">Required</span> when NOT using onboarding
{: .info }

CreateUser (bool)
: Create a user when adding a new employee - <span style="color: red">Required</span>

UserID
: The Employee ID of the employee - <span style="color: red">Required if creating a user</span>

Password
: The Employee ID of the employee - <span style="color: red">Required if creating a user</span>

RoleID
: The Role ID of the employee - <span style="color: red">Required if creating a user</span>

###### Example

```
https://{baseurl}/ClientAPI/CreateNewEmployee?token={token}&companyid=1&clientid=001
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
