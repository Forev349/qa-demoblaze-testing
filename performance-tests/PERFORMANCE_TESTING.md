## Scenario 1: Login Load Test / Тест нагрузки на вход

Endpoint:
POST https://api.demoblaze.com/login

---

Test Configuration / Настройки теста:
1. Virtual Users (VUs) / Виртуальные пользователи: 10
2. Duration / Длительность: 10 seconds

---

Results / Результаты:
1. Avg response time / Среднее время отклика: 13.83 s
2. Max response time / Максимальное время отклика: 13.92 s
3. Total requests / Всего запросов: 10
4. Error rate / Процент ошибок: 0%

---

Observations / Наблюдения:
1. All requests were successfully processed (status 200)
Все запросы успешно обработаны (код 200)
2. No server errors detected
Ошибок на стороне сервера не обнаружено
3. Response time is significantly higher than expected
Время отклика значительно выше ожидаемого

---

Issues / Проблемы:
1. High response time under load (>13 seconds)
Высокое время отклика при нагрузке (>13 секунд)
2. May negatively impact user experience
Может негативно повлиять на пользовательский опыт

---

Conclusion / Вывод:

The system remains stable under load but demonstrates poor performance due to high response time.
Система остаётся стабильной при нагрузке, но показывает низкую производительность из-за долгого времени отклика.

---

## Scenario 2: Signup Load Test / Тест нагрузки на регистрацию

Endpoint:
POST https://api.demoblaze.com/signup

---

Test Configuration / Настройки теста:
1. Virtual Users (VUs) / Виртуальные пользователи: 10
2. Duration / Длительность: 20 seconds

---

Results / Результаты:
1. Avg response time / Среднее время отклика: 0.69 s
2. Max response time / Максимальное время отклика: 2.63 s
3. Total requests / Всего запросов: 65
4. Error rate / Процент ошибок: 0%

---

Observations / Наблюдения:
1. All requests were successfully processed (status 200) /
Все запросы успешно обработаны (код 200) 
2. No server errors detected /
Ошибок на стороне сервера не обнаружено
3. Response time is mostly stable /
Время отклика в основном стабильное

---

Risks / Риски:
1. Occasional response time spikes (up to 2.63 s) /
Периодические скачки времени отклика (до 2.63 сек)
2. Performance may degrade under higher load /
Производительность может ухудшиться при большей нагрузке

---

Conclusion / Вывод:

The signup endpoint performs well under current load but shows potential risks due to response time spikes. /
Эндпоинт регистрации работает стабильно при текущей нагрузке, но есть риски из-за скачков времени отклика.
