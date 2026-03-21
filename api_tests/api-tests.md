## API Test 1:
User Login

Method: POST

URL: https://api.demoblaze.com/login

Body:{"username":"testuser","password":"hash"}

Expected Result:
Status code 200. User is authenticated succesfully

Ожидаемый результат:
Код состояния 200. Пользователь успешно прошел аутентификацию

Actul Result:
Status code: 200
The user is not logged in because the password is incorrect
The server returned a correct response of "Wrong password"

Результат проверки:
Код состояния: 200
Пользователь не вошел в систему, так как пароль не правильный
Сервер вернул корректный ответ "Wrong password"

Notes:
Request was tested using Postman
Backend correctly processes authentication request

Записи:
Запрос был протестирован с помощью Postman
Серверная часть корректно обрабатывает запрос на аутентификацию
