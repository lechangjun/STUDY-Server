# deterministic โ Delay and Rollback

deterministic โ ๋ณต์ต

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.53.48.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.53.48.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.53.55.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.53.55.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.54.21.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.54.21.png)

sync

desync

# ๐ Delay โ desyne ๋ง๋ ๋ฒ

latency  ์๊ฐ ๋งํผ Delay๋ฅผ ์ค์ sync๊ฐ ๋ง๋ ๋ฐฉ๋ฒ 

```bash
acme run --local
```

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.57.43.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.57.43.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.58.42.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.58.42.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.59.19.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.59.19.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.59.41.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__7.59.41.png)

๋ฌธ์ ์  : Delay ๊ฐ ์๊น ๋๋ฆฌ๊ฒ ํ๋์ด ์ผ์ด๋จ 

```bash
acme --help
```

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.03.21.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.03.21.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.05.30.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.05.30.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.07.28.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.07.28.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.09.53.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.09.53.png)

# ๐ข Rollback

ํ๋์ด ์ผ์ด๋ ๊ฐ์ ์ด์  ์๊ฐ์ ์ ์ฅํด์ sync ๋ฅผ ๋ง์ถ๋ ๋ฐฉ๋ฒ

```bash
acme deploy --staging 
```

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.12.21.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.12.21.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.13.14.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.13.14.png)

๋ฌธ์ ์ : ๋  ๋๋ฌธ์ด๋ค. ๋ ์ด ๊ฑธ๋ฆฐ๋ค๊ณ  ํ๋ ๊ฒฝ์ฐ๊ฐ rollback

       ๋ง๋ค๊ธฐ ์ด๋ ต๋ค. ์ค๊ฐ ์ ์ ์ฒ๋ฆฌ๊ฐ ์ด๋ ต๋ค.

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.15.38.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.15.38.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.16.44.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.16.44.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.21.41.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.21.41.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.23.28.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.23.28.png)

deterministic โ ๋ฌธ์ ์  : ์ค๊ฐ ์ ์ ์ฒ๋ฆฌ๊ฐ ์ด๋ ต๋ค.

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.24.50.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.24.50.png)

![deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.23.59.png](deterministic%20%E2%86%92%20Delay%20and%20Rollback%20f999a57919b34c5bbf14a69df618e2c8/_2021-07-17__8.23.59.png)