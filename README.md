# **ECSE3038 LAB 3**  

**This repo was created as part of a laboratory excersise that is meant to get students more accustomed to the technologies used in designing and implementing a RESTful API server with MongoDB service.**   

# **The three routes used and their operation is as follows:**

## **/profile**  

1. A user is allowed to create ONE profile consisting of Username, Role and Favorite color.  

2. A POST request allows the user to create a profile. The information provided is stored within a global variable in the script. Date and time is updated by the server with each request.  

3. The user is also allowed to make changes to the profile using a PATCH request consisting of a JSON body with any combination of the three attributes. Date and time are also updated by the server to show when the last update was made.  

4. A GET request returns a singular JSON object. Initial dummy values are set and are returned after a GET request if the user hasn't yet created a profile.

## **/data**  

1. An initial GET request returns an empty array from the database. After data has been added using the POST request, it returns the posted object in the array.

2. A POST request allows the user to add new tanks to the database for each of which an ID is automatically generated. 

## **/data/:id**  

1. The user can send a PATCH request to change the parts of one of the tanks after it has been posted to the database. The requester can make a JSON body with any combination of the attributes and update them as necessary. The "id" attribute cannot be edited.

2. The user can make a DELETE request to delete any previously POSTed object from the database by providing the id number of the object they wish to delete.






