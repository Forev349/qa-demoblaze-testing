## Scenario 1: Login Load Test 

## Scenario 1: Тест нагрузки на вход

Endpoint:
POST https://api.demoblaze.com/login

---

Test Configuration:

Настройки теста:

1. Virtual Users (VUs): 10
2. Duration: 10 seconds

1. Виртуальные пользователи: 10
2. Длительность: 10 seconds

---

Results:

Результаты:

1. Avg response time: 13.83 s
2. Max response time: 13.92 s
3. Total requests: 10
4. Error rate: 0%

1. Среднее время отклика: 13.83 s
2. Максимальное время отклика: 13.92 s
3. Всего запросов: 10
4. Процент ошибок: 0%

---

Observations:

Наблюдения:

1. All requests were successfully processed (status 200)
2. No server errors detected
3. Response time is significantly higher than expected

1. Все запросы успешно обработаны (код 200)
2. Ошибок на стороне сервера не обнаружено
3. Время отклика значительно выше ожидаемого

---

Issues:

Проблемы:

1. High response time under load (>13 seconds)
2. May negatively impact user experience

1. Высокое время отклика при нагрузке (>13 секунд)
2. Может негативно повлиять на пользовательский опыт

---

Conclusion: The system remains stable under load but demonstrates poor performance due to high response time.

Вывод: Система остаётся стабильной при нагрузке, но показывает низкую производительность из-за долгого времени отклика.

---

## Scenario 2: Signup Load Test / Тест нагрузки на регистрацию

Endpoint:
POST https://api.demoblaze.com/signup

---

Test Configuration:

Настройки теста:

1. Virtual Users (VUs): 10
2. Duration: 20 seconds

1. Виртуальные пользователи: 10
2. Длительность: 20 seconds

---

Results:

Результаты:

1. Avg response time: 0.69 s
2. Max response time: 2.63 s
3. Total requests: 65
4. Error rate: 0%

1. Среднее время отклика: 0.69 s
2. Максимальное время отклика: 2.63 s
3. Всего запросов: 65
4. Процент ошибок: 0%

---

Observations:

Наблюдения:

1. All requests were successfully processed (status 200)
2. No server errors detected
3. Response time is mostly stable

1. Все запросы успешно обработаны (код 200)
2. Ошибок на стороне сервера не обнаружено
3. Время отклика в основном стабильное

---

Risks:

Риски:

1. Occasional response time spikes (up to 2.63 s)
2. Performance may degrade under higher load

1. Периодические скачки времени отклика (до 2.63 сек)
2. Производительность может ухудшиться при большей нагрузке

---

Conclusion: The signup endpoint performs well under current load but shows potential risks due to response time spikes.

Вывод: Эндпоинт регистрации работает стабильно при текущей нагрузке, но есть риски из-за скачков времени отклика.

