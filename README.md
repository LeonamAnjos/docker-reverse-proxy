## docker-reverse-proxy
##### Proof of concept

Add the following lines to the `hosts` file:
```
127.0.0.1	web.my-domain.com
127.0.0.1	api.my-domain.com
```

Go to the root folder of the repo and load the containers:
```sh
$ cd ~/repos/docker-reverse-proxy
$ docker-compose up
```

Open your brownser and try the following urls:
- http://web.my-domain.com
- http://api.my-domain.com
