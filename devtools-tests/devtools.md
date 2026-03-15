## DevTools Test 1: Registration request

## DevTools тест 1: Запрос регистрации

Preconditions:
User does not have an account on the website.

Предусловия:
У пользователя нет аккаунта на сайте.

Steps / Шаги:
 1. Open Chrome DevTools (F12) / Открыть Chrome DevTools (F12)
 2. Go to the Network tab / Перейти на вкладку Network
 3. Perform registration on https://www.demoblaze.com / Зарегистрировать нового пользователя на сайте
 4. Find the registration POST request in the Network tab / Найти POST-запрос регистрации
 5. Check status code and response / Проверить код ответа и ответ сервера

Expected Result / Ожидаемый результат:
Request status code is 200 and server returns success message / Код ответа 200, сервер возвращает сообщение об успешной регистрации

Actual Result / Фактический результат:
Request status code is 200 and server returns success message / Код ответа 200, сервер возвращает сообщение об успешной регистрации

Notes / Примечания:
Even though the UI test passed, this confirms that the backend received the registration data correctly / Даже если UI тест прошёл, это подтверждает, что бэкенд получил данные регистрации корректно

---



