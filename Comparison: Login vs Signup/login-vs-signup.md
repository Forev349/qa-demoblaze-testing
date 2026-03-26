## Performance Comparison / Сравнение производительности

---

Key Metrics / Основные метрики:

| Metric | Login | Signup |
|--------|------|--------|
| Avg response time | 13.83 s | 0.69 s |
| Max response time | 13.92 s | 2.63 s |
| Error rate | 0% | 0% |
| Total requests | 10 | 65 |

---

## Analysis / Анализ:

EN:

Login endpoint shows significantly worse performance compared to signup.
While signup handles requests efficiently, login response time is extremely high (~13s), which indicates a potential backend bottleneck.

RU:

Эндпоинт входа показывает значительно худшую производительность по сравнению с регистрацией.
Регистрация работает быстро, а вход занимает ~13 секунд, что может указывать на узкое место на стороне сервера.

---

## Key Finding / Главный вывод

EN:

Different endpoints demonstrate inconsistent performance under similar load conditions.

RU:

Разные эндпоинты показывают нестабильную производительность при одинаковой нагрузке.

---

## Recommendations / Рекомендации

**EN:**

- Investigate backend logic of the login endpoint  
- Optimize authentication process to reduce response time  
- Analyze database queries and server load handling  

**RU:**

- Проверить логику backend для login  
- Оптимизировать процесс авторизации для уменьшения времени отклика  
- Проанализировать запросы к базе данных и обработку нагрузки  
