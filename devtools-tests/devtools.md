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
1. Open https://www.demoblaze.com
2. Click “Sign up”
3. Leave username field empty
4. Leave password field empty
5. Click “Sign up”

Шаги:
1. Откройте https://www.demoblaze.com
2. Нажмите «Зарегистрироваться»
3. Оставьте поле «Имя пользователя» пустым
4. Оставьте поле «Пароль» пустым
5. Нажмите «Зарегистрироваться»

Expected Result:
System should display validation message for required fields.
No request should be sent to the server.

Ожидаемый результат:
Система должна отображать сообщение об ошибке проверки для обязательных полей.
Запросы на сервер отправляться не должны.

Actual Result:
Validation message is displayed and no network request is sent.

Результат:
Отображается сообщение об ошибке проверки, и сетевой запрос не отправляется.

Notes:
Form validation is handled on the client side before sending any network request.

Примечания:
Проверка формы выполняется на стороне клиента перед отправкой любого сетевого запроса.

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

Expected Result: System should display an error message “Wrong password”.

Ожидаемый результат:
Система должна отображать сообщение об ошибке «Неверный пароль».

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
1 Open https://www.demoblaze.com
2 Click “Log in”
3 Leave fields empty
4 Click “Log in”

Шаги:
1. Откройте https://www.demoblaze.com
2. Нажмите «Войти»
3. Оставьте поля пустыми
4. Нажмите «Войти»

Expected Result: 
System should display validation messages for required fields and no request should be sent to the server.

Ожидаемый результат: 
Система должна отображать сообщения об ошибке для обязательных полей, запрос на сервер не должен отправляться.

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
System should add the product to the cart and return status code 200.

Ожидаемый результат:
Товар добавится в корзину

Actual Result:
The server responded that the product was added to the cart and that a successful POST request was received (code 200)

Результат:
Сервер отправил ответ, что продукт был добавлен в корзину, а также присутствует успешный POST-запрос (код 200)

---

## Test Case 8: Remove product from cart

## Тест-кейс 8: Удаление товара из корзины

Preconditions: User has at least one product in the cart.

Предусловия: В корзине есть хотя бы один товар.

Steps:
 1. Open Chrome DevTools (F12)
 2. Go to the Network tab
 3. Remove an item from the shopping cart
 4. Find the DELETE request
 5. Check status code and response

Шаги:
 1. Открыть Chrome DevTools (F12)
 2. Перейти на вкладку Network
 3. Убрать товар из корзины
 4. Найти DELETE-запрос
 5. Проверить код ответа и ответ сервера

Expected Result:
The product will be removed from the basket.

Ожидаемый результат:
Товар будет убран из корзины

Actual Result: Product was successfully removed from the cart. Server returned status code 200.

Результат: Товар успешно удалён из корзины, сервер вернул код 200.

---

## Test Case 9: Place an order

## Тест-кейс 9: Оформление заказа

Preconditions: User has at least one product in the cart and is logged in.

Предусловия: В корзине есть хотя бы один товар, пользователь вошёл в аккаунт.

Steps:
 1. Open Chrome DevTools (F12)
 2. Go to the Network tab
 3. Place an order
 4. Find a POST request
 5. Check status code and response

Шаги:
 1. Открыть Chrome DevTools (F12)
 2. Перейти на вкладку Network
 3. Сделать заказ
 4. Найти POST-запрос
 5. Проверить код ответа и ответ сервера

Expected Result:
System should successfully place the order and return status code 200.

Ожидаемый результат:
Система должна успешно оформить заказ и вернуть код ответа 200.

Actual Result:
The server responded with information about the order and a successful POST 200 request

Результат:
Пришел ответ сервера, в котором написана информация о заказе, а так же успешно отправлен запрос POST 200
