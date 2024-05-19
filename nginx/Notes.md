# Creating NGINX Conf Files
- Located in `/etc/nginx` (or other for open source nginx)
- Directives:
```
user foo;
error_log bar notice;
worker_processes 1;
```
- Recommendation:
    - Break into features inside: `/etc/nginx/conf.d`:
```
include conf.d/http;
include conf.d/stream;
include conf.d/exchange-enhanced;
```
- Contexts:
TODO
- Virtual Servers:
    - Inside context blocks:
```
http {
    server {
        ...
    }
}
stream {
    server {
        ...
    }
}
```


