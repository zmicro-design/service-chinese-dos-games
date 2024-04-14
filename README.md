# Chinese DOS Games Service

## Getting Start

- 1. Start service with zmicro

```shell
$ zmicro service start chinese-dos-games
```

- 2. Download games

```shell
# Download all games
$ zmicro service exec chinese-dos-games python3 /app/static/games/download_data.py

# If cannot download, maybe your network error, use HTTP_PROXY
$ zmicro service exec chinese-dos-games
$ HTTPS_PROXY=http://<YOUR_PROXY_HOST>:<YOUR_PROXY_PORT> python3 /app/static/games/download_data.py
```

- 3. Open browser

```shell
$ open http://localhost:5000
```
