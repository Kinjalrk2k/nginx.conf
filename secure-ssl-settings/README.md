### Secure SSL settings
- Disable SSLv3 which is enabled by default. This prevents [POODLE SSL Attack](http://nginx.com/blog/nginx-poodle-ssl/).
- Ciphers that best allow protection from Beast. [Mozilla Server Side TLS and Nginx]( https://wiki.mozilla.org/Security/Server_Side_TLS#Nginx)