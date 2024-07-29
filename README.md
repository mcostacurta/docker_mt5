
# MetaTrader 5 on Docker environment

An easily way to set up a MetaTrader 5 environment usig Docker, it can be used to develop on Python or use MetaTrader over Browser.


## Use

1. Clone the repo

```bash 
git clone <repo>
```

2. Execute
```bash
docker-compose up -d
```

3. Access
```bash

4. Conect using web interface

```bash
http://localhost:3000
```
5. Execute a python script to test (on host machine)

```python
from mt5linux import MetaTrader5
mt5 = MetaTrader5(host='localhost',port=8001)
mt5.initialize()
print(mt5.version())
```

You should see somehitng like this

```
(500, 4461, '28 Jul 2024')
```


These repo was created based on the repo: https://github.com/gmag11/MetaTrader5-Docker-Image/tree/main?tab=readme-ov-file