## Scenario 1: Login Load Test

Endpoint:
POST https://api.demoblaze.com/login

Test Configuration:
1. Virtual Users: 10
2. Duration: 10 seconds

Result:
1. Avg response time: 13.83 s
2. Max response time: 13.92 s
3. Error rate: 0%
4. Total requests: 10

Observations:
1. All requests were seccesfully processed (status 200)
2. No server errors defected
3. Response time is significantly higher than expected

Issue:
1. High response time under load (>13 seconds)
2. May negatively impact user experience

Conclusion:
The system remains stable under load but demonstrates poor performance due to high response time

## Scenario 2: Signup Load Test

Endpoint:
POST https://api.demoblaze.com/signup

Test Configuration:
1. Virtual Users: 10
2. Duration: 20 seconds

Result:
1. Avg response time: 0.69 s
2. Max response time: 2.63 s
3. Total requests: 65
4. Error rate: 0%

Observations:
1. All requests were seccesfully processed (status 200)
2. No server errors defected
3. Response time is mostly stable

Risks:


