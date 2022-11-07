# API Testing
* Api testing is the frontend and the database communicate to each other they are not directly communicate middle sight the server work and the api serve the data frontend to the database and get the data from database to the frontend and show the information.
* Using Postman for API tesing
* Report Generate using the NewMan ( Globali Install the Newman) 
<!DOCTYPE html>
<html>
<head>
</head>
<body>
 <h1>How done by the api testing</h1>
  * First Create the collection <br>
  * Then create the add request option <br>
  * Using the Method (Post, Get, Put and Delete) <br>
  * Post Method Use Insert the Data <br>
  * Get Method Use get the specific user by the id number <br>
  * Put method updated the specific information using by id
  * delete method delete the specific user using by the id
  <h1>Using the Test Option in postman</h1>
  * Crate the Enviormen <br>
  * the test option write the javascript code and every api used variable send to the environment and use this data dynamically <br>
  * Write the Test Case in Test option <br>
  * checking the data are wrong or correct <br>
  var jsonData = pm.response.json()

pm.environment.set("id", jsonData.bookingid)

var code = responseCode.code
console.log(code)

switch(code){
    case 200:

    pm.test("first name", function(){
        pm.expect(jsonData.booking.firstname).to.equal(pm.environment.get("firsname"))
    })

    break;

    default:
} 
<br>

* Using the Pre-request Script
<h1>Newman</h1>
  
</body>
</html>
