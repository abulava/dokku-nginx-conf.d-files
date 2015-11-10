# dokku-nginx-conf.d-files

Simple management of files in nginx.conf.d directory for an application. Nginx will include any file from that directory if its filename matches *.conf pattern. Besides, you can use it to put a file with trusted CA certificates in the PEM format used to verify client certificates and OCSP responses, then refer it in "ssl_trusted_certificate" directive and enable [ssl_stapling][ssl_stapling].

## Installation

```sh
# dokku 0.4+
dokku plugin:install https://github.com/abulava/dokku-nginx-conf.d-files.git
```

## License

This plugin is released under the MIT license. See the file [LICENSE](LICENSE).

[ssl_stapling]: http://nginx.org/en/docs/http/ngx_http_ssl_module.html#ssl_stapling
