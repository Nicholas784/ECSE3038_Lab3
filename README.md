# **ECSE3038 LAB 3**  

## **This is a modification of the previous RESTful API now with MongoDB service to add, remove and modify tanks to/from a database.**   

### **The routes that were edited are shown below with the changes made to accomodate the mongoDB service:**

## **/data**  

1. An initial GET request returns an empty array from the database. After data has been added using the POST request, it returns the posted object in the array.

2. A POST request allows the user to add new tanks to the database for each of which an ID is automatically generated. 

## **/data/id**  

1. The user can send a PATCH request to change the parts of one of the tanks after it has been posted to the database. The requester can make a JSON body with any combination of the attributes and update them as necessary. The "id" attribute cannot be edited.

2. The user can make a DELETE request to delete any previously POSTed object from the database by providing the id number of the object they wish to delete.






