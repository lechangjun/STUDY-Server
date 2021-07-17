# deterministic → Delay and Rollback

deterministic → 복습

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.53.48.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.53.48.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.53.55.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.53.55.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.54.21.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.54.21.png)

sync

desync

# 🚚 Delay → desyne 막는 법

latency  시간 만큼 Delay를 줘서 sync가 맞는 방법 

```bash
acme run --local
```

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.57.43.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.57.43.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.58.42.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.58.42.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.59.19.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.59.19.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.59.41.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.59.41.png)

문제점 : Delay 가 생김 느리게 행동이 일어남 

```bash
acme --help
```

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.03.21.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.03.21.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.05.30.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.05.30.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.07.28.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.07.28.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.09.53.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.09.53.png)

# 🚢 Rollback

행동이 일어난 값을 이전 시간에 저장해서 sync 를 맞추는 방법

```bash
acme deploy --staging 
```

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.12.21.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.12.21.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.13.14.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.13.14.png)

문제점: 렉 때문이다. 렉이 걸린다고 하는 경우가 rollback

       만들기 어렵다. 중간 접속 처리가 어렵다.

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.15.38.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.15.38.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.16.44.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.16.44.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.21.41.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.21.41.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.23.28.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.23.28.png)

deterministic → 문제점 : 중간 접속 처리가 어렵다.

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.24.50.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.24.50.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.23.59.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.23.59.png)