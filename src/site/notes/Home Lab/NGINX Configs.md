---
{"dg-publish":true,"permalink":"/home-lab/nginx-configs/"}
---


```sh
server {
    listen              443 **ssl**;
    server_name         www.example.com;
    ssl_certificate     **www.example.com.crt**;
    ssl_certificate_key **www.example.com.key**;
    ssl_protocols       TLSv1 TLSv1.1 TLSv1.2 TLSv1.3;
    ssl_ciphers         HIGH:!aNULL:!MD5;
    ...
```

