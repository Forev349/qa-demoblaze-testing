## API Test 1:
Valid login

Method:
POST

URL:
https://api.demoblaze.com/login

Body:
{"username":"Gordey003","password":"hash"}

Expected Result:
1. Status code: 200 OK
1. Logged in to the account

Actual Result:
The user has successfully logged into the account

---

## API Test 2:
Wrong password

Method:
POST

URL: 
https://api.demoblaze.com/login

Body:
{"username":"testuser","password":"123"}

Expected Result:
1. Status code 200 OK
2. User is NOT authenticated

Actul Result:
1. Status code: 200 OK
2. Response body: "Wrong password"

---

## API Test 3:
wrong username

Method:
POST

URL:
https://api.demoblaze.com/login

Body:
{
"username": "Gordey007", 
"password": "TWFsb3kyMDA3"
}

Expected Result:
1. Status code: 200 OK
2. User is NOT authenticated

Actual Result:
1. Status code: 200 OK
2. Response body: "User does not exist."

---

## API Test 4:
empty username

Method:
POST

URL: 
https://api.demoblaze.com/login

Body:
{"username":"","password":"123"}

Expected Result:
1. Status code: 400 Bad Request - validation error
2. User is NOT authenticated
3. The server should not break down

Actul Result:
1. Status code: 500 Internal Server Error
2. Response body: "Please fill out Username and Password"

Conclusion: Bug detected

---

API Test 5:
empty password

Method:
POST

URL: 
https://api.demoblaze.com/login

Body:
{"username":"Gordey003","password":""}

Expected Result:
1. Status code: 200
2. User is NOT authenticated
3. Response body: "Wrong password."

Actul Result:
2. Status code: 200
1. Response body: "Wrong password."

---

API Test 6:
empty body

Method:
POST

URL:
https://api.demoblaze.com/login

Body:
{}

Expected Result:
1. Request should be validated
2. User should NOT be authenticated
3. The server should not break down

Actual Result:
1. Status code: 200
3. Response body: "Bad parameter, missing username"}

---

API Test 7:
SQL injection

Method:
POST

URL:
https://api.demoblaze.com/login

Body:
{"username":"' OR 1=1 --'","password":"MTIz"}

Expected Result:
1. Status code: 200
2. User is NOT authenticated
3. The server should not break down

Actual result:
1. Status code: 200
2. Response body: "User does not exist."
