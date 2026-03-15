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

Expected Result:
Response code 200, the server returns a message indicating that the user has already been created

Ожидаемый результат:
Код ответа 200, сервер возвращает сообщение о том, что пользователь уже создан

Actual Result:
Response code 200, the server returns a message indicating that the user has already been created ("his user already exist")

Результат:
Код ответа 200, сервер возвращает сообщение о том, что пользователь уже создан

Notes:
Code 200 is normal because the POST request successfully reached the server. The server correctly responded that the user already exists.

Примечания:
Код 200 это норма, так как POST-запрос успешно дошёл до сервера, который вернул корректный ответ, что пользователь уже существует.

---

## Test Case 3: Registration with empty fields

## Тест-кейс 3: Регистрация с пустыми полями

Preconditions: User opens the registration form.

Предусловия: Пользователь открыл форму регистрации.

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

Expected Result:
The server returns a message requiring input data

Ожидаемый результат:
Сервер возвращает сообщение о требовании ввода данных

Actual Result:
The server returns a message asking for Username and Password

Результат:
сервер возвращает сообщение о требовании ввода Username и Password

Notes:
There is no response code, as validation occurs on the client side before the request is sent to the server.

Примечания:
Код ответа отсутствует, так как валидация происходит на стороне клиента до отправки запроса на сервер.

---

## Test Case 4: Login with valid credentials

## Тест-кейс 4: Вход с корректными учетными данными

Preconditions: User has a registered account on DemoBlaze.

Предусловия: У пользователя есть зарегистрированный аккаунт на DemoBlaze.

Steps:
 1. Open Chrome DevTools (F12)
 2. Go to the Network tab
 3. Try logging into the created account (https://www.demoblaze.com)
 4. Find the Login POST request
 5. Check status code and response

Шаги:
 1. Открыть Chrome DevTools (F12)
 2. Перейти на вкладку Network
 3. Попробовать войти в созданный аккаунт
 4. Найти POST-запрос входа
 5. Проверить код ответа и ответ сервера

Expected Result:
Response code 200 (POST), successfully logged in to the account

Ожидаемый результат:
Код ответа 200 (POST), успешно зашел на аккаунт

Actual Result:
Response code 200, logged in to the account

Результат:
Код ответа 200, получилось зайти в аккаунт

Notes:
The login process includes two successful requests:
 • POST request (Check) – sends the username and password to the server for authentication.
 • GET request – retrieves the user's data after successful login.
Both requests returned a 200 code, indicating that the server successfully processed the requests and the user's account was loaded correctly.

Примечания:
Процесс входа включает два успешных запроса:
 • POST запрос (Check) – отправляет имя пользователя и пароль на сервер для аутентификации.
 • GET запрос – получает данные пользователя после успешного входа.
Оба запроса вернули код 200, что означает, что сервер успешно обработал запросы и аккаунт пользователя был корректно загружен.

---

## Test Case 5: Login with invalid password

## Тест-кейс 5: Вход с неправильным паролем

Preconditions: User has a registered account on DemoBlaze.

Предусловия: У пользователя есть зарегистрированный аккаунт на DemoBlaze.

Steps:
 1. Open Chrome DevTools (F12)
 2. Go to the Network tab
 3. Try logging into the created account (https://www.demoblaze.com)
 4. Find the Login POST request
 5. Check status code and response

Шаги:
 1. Открыть Chrome DevTools (F12)
 2. Перейти на вкладку Network
 3. Попробовать войти в созданный аккаунт
 4. Найти POST-запрос входа
 5. Проверить код ответа и ответ сервера

Expected Result:
The system displays an error message saying "Invalid password", but there will be a 200(POST) code, as the information must reach the server

Ожидаемый результат:
Система показывает сообщение об ошибке «Неверный пароль», но будет код 200(POST), так как информация должна дойти до сервера

Actual Result:
Response code 200(POST), error message "Wrong password"

Результат:
Код ответа 200(POST), сообщение об ошибке "Неверный пароль"

---

## Test Case 6: Login with empty fields

## Тест-кейс 6: Вход с пустыми полями

Preconditions: User opens the login form on DemoBlaze.

Предусловия: Пользователь открыл форму входа на DemoBlaze.

Steps:
 1. Open Chrome DevTools (F12)
 2. Go to the Network tab
 3. Try logging in to your account (https://www.demoblaze.com)
 4. Find the Login POST request
 5. Check status code and response

Шаги:
 1. Открыть Chrome DevTools (F12)
 2. Перейти на вкладку Network
 3. Попробовать войти в аккаунт
 4. Найти POST-запрос входа
 5. Проверить код ответа и ответ сервера

Expected Result:
The system shows an error message

Ожидаемый результат:
Система показывает сообщение об ошибке

Actual Result:
There is no response code, as validation occurs on the client side before the request is sent to the server.

Результат:
Код ответа отсутствует, так как валидация происходит на стороне клиента до отправки запроса на сервер.

---

## Test Case 7: Add product to cart

## Тест-кейс 7: Добавление товара в корзину

Preconditions: User is logged in.

Предусловия: Пользователь вошёл в аккаунт.

Steps:
 1. Open Chrome DevTools (F12)
 2. Go to the Network tab
 3. Add an item to the cart
 4. Find a POST request
 5. Check status code and response

Шаги:
 1. Открыть Chrome DevTools (F12)
 2. Перейти на вкладку Network
 3. Добавить товар в корзину
 4. Найти POST-запрос
 5. Проверить код ответа и ответ сервера

Expected Result:
The product will be added to the cart

Ожидаемый результат:
Товар добавится в корзину

Actual Result:
There is no response code, as validation occurs on the client side before the request is sent to the server.

Результат:
Код ответа отсутствует, так как валидация происходит на стороне клиента до отправки запроса на сервер.
