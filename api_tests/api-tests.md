## API Test 1:
User Login

Method:
POST

URL: 
https://api.demoblaze.com/login

Body:
{"username":"testuser","password":"hash"}

Expected Result:
1. User in not authenticated
2. Response contains "Wrong password"

Ожидаемый результат:
1. Пользователь не прошел проверку подлинности
2. В ответе содержится сообщение "Неверный пароль"

Actul Result:
1. Status code: 200
2. Response body: "Wrong password"
3. Response returned successfully

Результат проверки:
1. Код состояния: 200
2. Пользователь не вошел в систему, так как пароль не правильный
3. Ответ возвращен успешно

Notes:
1. Request was tested using Postman
2. Backend correctly processes authentication request

Записи:
1. Запрос был протестирован с помощью Postman
2. Серверная часть корректно обрабатывает запрос на аутентификацию
