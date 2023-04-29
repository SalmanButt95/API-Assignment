# API-Assignment

1. Get authentication token using URI: https://postman-echo.com/basic-auth
   Question: How did you get the response?

ANS:
![img.png](img.png)


2. Get information about all users using URI: https://reqres.in/api/users
   Question: How many lists can you see in the response body?

ANS: Only one list named "data"

![img_2.png](img_2.png)

3. Get information about the user with id 3 using URI: https://reqres.in/api/users/3
   Question: How many lists can you see in the response body? What are the available property(Key) names in the response body?

ANS: There's no list. There are 2 primary keys: "data" and "support". However, under 'data' primary keys, there are 5 keys which are :(id, email, first_name, last_name, and avatar). "Support" primary have two keys: (url, and text). In total there are two primary keys, or 9 keys within this response

![img_3.png](img_3.png)




4. Delete the User with id 9 using URI https://reqres.in/api/users/9
   Question: What is the response? How many users are now on the users list? https://reqres.in/api/users. Can you see the deleted user record?

ANS: Status 204 No Content. No response in body. 12 users. No able to delete user with id 9. (Failed)
![img_4.png](img_4.png)

5. Get information of the user with id 40 using URI: https://reqres.in/api/users/40
   Question: How many lists can you see in the response body? What are the available property(Key) names in the response body?

ANS: No list in response body, and no keys.
![img_5.png](img_5.png)



6. Create a new user in a system using URI: https://reqres.in/api/users Verb: POST Request Body:

        { 
          "name": "yourname",  
          "job": "dreamjob"
        }


Question: What is the response code? What are the available property(Key) names in the response body? What is the value of response Header Etag?

ANS: There are 4 keys in response body: (name, job, id, and createdAt). Etag is posted in picture below.

![img_6.png](img_6.png)
![img_7.png](img_7.png)



7. Sign in to the system using URI: https://reqres.in/api/login and {"email": "peter@klaven"}
   Question: What is the response code?


ANS: Response code 400 Bad Request. Error is missing password

![img_8.png](img_8.png)

8. Sign in to the system using URI: https://reqres.in/api/login and
   {
   "email": "eve.holt@reqres.in",
   "password": "cityslicka"
   }

Question: What is the value of response Header Etag? What is the response?

ANS: Response Staus is 200 OK. Response generated a "token". Etag is displayed in photo below
![img_9.png](img_9.png)
![img_10.png](img_10.png)



9. Get information about all planets using URI: https://swapi.dev/api/planets. Carefully observe the response body and make a list of all attributes and write their data types.
   Question: How many lists can you see in the response body?

ANS: The primary key has one list: "results". Under "results" list, every object has two lists (residents, and films)

![img_11.png](img_11.png)


10. Get information about the third planet using URI: https://swapi.dev/api/planets/3/
    Question: How many properties you can see in response body?

ANS: There are 12 Properties in the response body

![img_12.png](img_12.png)



11. Get information about all the starships using URI: https://swapi.dev/api/starships. Carefully observe the response body and make a list of all attributes and write their data types.
    Question:How many lists can you see in the response body?

ANS: The primary key has one list: "results". Under "results" list, every object has two lists (pilots, and films)

![img_13.png](img_13.png)


12. Get information about the ninth starship using URI: https://swapi.dev/api/starships/9/
    Question:How many lists can you see in the response body?

ANS: There is no primary key or list, but there are two object lists/array (pilots, and films)

![img_14.png](img_14.png)

13. Get information about all films using URI: https://swapi.dev/api/films. Carefully observe the response body and make a list of all attributes and write their data types.
    Question:How many lists can you see in the response body?

ANS: Primary list is "results", and object lists/array are 5 (characters, planets, starships, vehicles, and species).

![img_15.png](img_15.png)

14. Get information about the third planet using URI: https://swapi.dev/api/species
    Question:How many lists can you see in the response body?

ANS: Primary list is "results, and object lists/array are 2 (people, and films).

![img_16.png](img_16.png)



15. Get all booking ids using URI: https://restful-booker.herokuapp.com/booking
    Question: How many lists can you see in the response body?

ANS: No list

![img_17.png](img_17.png)



16. Get details about booking id 23 using URI: https://restful-booker.herokuapp.com/booking/23
    Question: What is the response?

![img_18.png](img_18.png)


17. Get details about booking id 3 using URI: https://restful-booker.herokuapp.com/booking/3
    Question: What is the response?

ANS: ![img_19.png](img_19.png)

18. Get information about all planets using URI: https://swapi.dev/api/planets
    Question: What is the response? How many lists can you see in the response body?

ANS: The primary key has one list: "results". Under "results" list, every object has two lists (residents, and films)

![img_20.png](img_20.png)

19. Get information about all species using URI: https://swapi.dev/api/species. Carefully observe the response body and make a list of all attributes and write their data types.
    Question: How many lists can you see in the response body? What is the response?

ANS: Primary list is "results, and object lists/array are 2 (people, and films).

![img_21.png](img_21.png)





20. Write JSON path for following JSON file:
    {
    "studio": {
    "movie": [
    {
    "category": "history",
    "director": "John",
    "title": "History",
    "rating": 6.60
    },
    {
    "category": "comedy",
    "director": "Paul",
    "title": "Laugh",
    "rating": 4.00
    },
    {
    "category": "fiction",
    "director": "Jack",
    "title": "Wake",
    "isbn": "87877676879",
    "rating": 8.01
    },
    {
    "category": "drama",
    "director": "Edward",
    "title": "Wuthering Heights",
    "isbn": "8754543578",
    "rating": 4.50
    }
    ],
    "music": {
    "song": "pale",
    "rate": 5.4
    }
    },
    "ranking": 20
    }

a. To retrieve all direct properties of the studio object

b. To find out the music’s song

c. To find the rating of all items in the studio

d. To retrieve information on all movies

e. To find out the titles of all movies

f. To retrieve the titles of all movies by Jack

g. To retrieve the category of the last movie

i. To retrieve all movies that have the isbn property

ANS: 

![img_22.png](img_22.png)



21. Get information about all employess using URI: http://dummy.restapiexample.com/api/v1/employees
    Question: How many lists can you see in the response body? What is the response? What are the available property(Key) names in the response body? Make a list of all attributes and write the data types.

ANS: One list called "data". There are 5 property keys (id (number), employee_name (string), employee_salary (number), employee_age (number), and profile_image (string)).

![img_23.png](img_23.png)

22. Get a single employee data using URI: http://dummy.restapiexample.com/api/v1/employee/3
    Question:How many data you can see in response body? What is the response status?

ANS: In the data bracket, there are properties such as: (id (number), employee_name (string), employee_salary (number), employee_age (number), and profile_image (string)). Response status is 200 OK

![img_24.png](img_24.png)

23. Create a new employee in a system by using URI: http://dummy.restapiexample.com/api/v1/create Verb: POST Request Body:
    {
    "name":"your name",
    "salary":"123",
    "age":"23"
    }

Question: What is the response? can you see "id" property in the response? if Yes, note the "id" value.


ANS: ![img_25.png](img_25.png)

24. Delete an employee record whose employee id in 2 by using URI http://dummy.restapiexample.com/api/v1/delete/2
    Question: What is the response? How many employees are now in the employees list? http://dummy.restapiexample.com/api/v1/employees. Can you see the deleted employee record?

ANS: 

![img_26.png](img_26.png)

25. Register a user by using URI: https://reqres.in/api/register Verb: POST Request Body:
    {
    "email": "john.jack@example.com",
    "password": "@izaanSchool"
    }

Question:What is the response? What are the available property(Key) names in the response body?


ANS: ![img_27.png](img_27.png)

26. Get an user Using URL https://reqres.in/api/unknown/2

Question: What is the response?

ANS: ![img_28.png](img_28.png)


27. A simple health check endpoint to confirm whether the API is up and running using https://restful-booker.herokuapp.com/ping
    Question: What is the response?

ANS: ![img_29.png](img_29.png)

28. Get information using Delayed Response using URI: https://reqres.in/api/users?delay=3


Question: What is the response? How many seconds delay to respond?

ANS: Response delay is 3.19s

![img_30.png](img_30.png)




29. Get information about vehicles using URL https://swapi.dev/api/vehicles/schema/
    Question: What type of response it is? What is response status code?

ANS: STATUS CODE IS 404 NOT FOUND. JSON response

![img_31.png](img_31.png)

30. Get information about starships using URL https://swapi.dev/api/starships/schema/
    Question: What type of response it is? Write down the response status code. What are the available property(Key) names in the response body?

ANS: STATUS CODE IS 404 NOT FOUND. JSON response. No keys.

![img_31.png](img_31.png)