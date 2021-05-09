# docker-reverse-proxy
## Introduction
Proof of concept using docker nginx to redirect https requests to different sites in the same server.

The folder `proxy` contains the nginx configuration that will receive `http` or `https` requestes and will proxy to the correct site.

The folders app1 and app2 contain the sites that will receive http requests from the proxy.
## Prerequisites
- [Docker engine](https://docs.docker.com/engine/install/)
## Setup
### Hosts
Add the following lines to the `hosts` file:
```
127.0.0.1	web.my-xyz-domain.com
127.0.0.1	api.my-xyz-domain.com
```
## Run
Go to the root folder of the repo and load the containers:
```sh
$ cd ~/repos/docker-reverse-proxy
$ docker-compose up
```
Open your brownser and try the following urls:
- http://web.my-xyz-domain.com
- http://api.my-xyz-domain.com
