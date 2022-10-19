
This repository is used to deploy WordPress on kubernetes.

The ![Dockerfile.siege](./Dockerfile.siege) can be used to stress on WordPress as benchmark client

Usage: 
```
# build docker image
docker build -t siege -f Dockerfile.siege .

# run container
docker run -it siege -c 100 -t 60S http://<wordpress_ip>:<wordpress_port>

```


