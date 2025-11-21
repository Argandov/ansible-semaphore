# Setup

For the env var `SEMAPHORE_ACCESS_KEY_ENCRYPTION`, create it with:

``` bash
head -c32 /dev/urandom | base64
```

And never rotate it. 

```bash
mv env.example .env
```

Configure the environment variables' file

```bash
docker compose up -d
```

Login to the server's UI via:

`http://<server-ip>:3000`
