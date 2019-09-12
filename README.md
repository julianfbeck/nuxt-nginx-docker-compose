# nuxt-nginx-docker-compose

> Run a nuxt website with nginx and https

This docker-compose [jwilder/nginx-proxy](https://github.com/jwilder/nginx-proxy) and [jrcs/docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) containers to host a nuxt website. 
The Dockerfile to host the nuxt site is in the *app/* directory

## Setup
Replace following fields with your domain and email.
```yml
environment:
- VIRTUAL_HOST=yourdomain.com 
- LETSENCRYPT_HOST=yourdomain.com
- LETSENCRYPT_EMAIL=your@mail.com
```


## Usage
```
docker-compose up -d 
```

## Based on
- [jwilder/nginx-proxy](https://github.com/jwilder/nginx-proxy) 
- [jrcs/docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) 
- [Nextclouds docker-compose](https://github.com/nextcloud/docker/tree/master/.examples)
