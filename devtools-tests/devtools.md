## DevTools Test 1: Registration request

## DevTools тест 1: Запрос регистрации

Preconditions:
User does not have an account on the website.

Предусловия:
У пользователя нет аккаунта на сайте.

Steps:
 1. Open Chrome DevTools (F12)
 2. Go to the Network tab
 3. Perform registration on https://www.demoblaze.com
 4. Find the registration POST request in the Network tab
 5. Check status code and response

Шаги:
 1. Открыть Chrome DevTools (F12)
 2. Перейти на вкладку Network
 3. Зарегистрировать нового пользователя на сайте
 4. Найти POST-запрос регистрации
 5. Проверить код ответа и ответ сервера

Expected Result:
Request status code is 200 and server returns success message

Ожидаемый результат:
Код ответа 200, сервер возвращает сообщение об успешной регистрации

Actual Result:
Request status code is 200 and server returns success message

Результат:
Код ответа 200, сервер возвращает сообщение об успешной регистрации

Notes:
Even though the UI test passed, this confirms that the backend received the registration data correctly

Примечания:
Даже если UI тест прошёл, это подтверждает, что бэкенд получил данные регистрации корректно

---

## DevTools Test 2: Registration with existing username

## DevTools тест 2: Регистрация с уже существующим именем пользователя

Preconditions: A user with this username already exists.

Предусловия: Пользователь с таким именем уже зарегистрирован.

Steps:
 1. Open Chrome DevTools (F12)
 2. Go to the Network tab
 3. Try to register an account that has already been created (https://www.demoblaze.com)
 4. Find the registration POST request in the Network tab
 5. Check status code and response

Шаги:
 1. Открыть Chrome DevTools (F12)
 2. Перейти на вкладку Network
 3. Попробовать зарегистрировать уже созданный аккаунт
 4. Найти POST-запрос регистрации
 5. Проверить код ответа и ответ сервера
