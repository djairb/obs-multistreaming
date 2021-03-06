nginx-rtmp-win32
================

* Nginx: 1.17.10 
* Nginx-Rtmp-Module: https://github.com/arut/nginx-rtmp-module
* openss1.1.1g
* pcre-8.44
* zlib-1.2.11

# configure arguments
```
auto/configure \
--with-cc=cl \
--builddir=build \
--with-debug \
--prefix= \
--conf-path=conf/nginx.conf \
--pid-path=logs/nginx.pid \
--http-log-path=logs/access.log \
--error-log-path=logs/error.log \
--sbin-path=nginx.exe \
--http-client-body-temp-path=temp/client_body_temp \
--http-proxy-temp-path=temp/proxy_temp \
--http-fastcgi-temp-path=temp/fastcgi_temp \
--http-scgi-temp-path=temp/scgi_temp \
--http-uwsgi-temp-path=temp/uwsgi_temp \
--with-cc-opt=-DFD_SETSIZE=1024 \
--with-pcre=objs/lib/pcre-8.44 \
--with-zlib=objs/lib/zlib-1.2.11 \
--with-openssl=objs/lib/openssl-1.1.1g \
--with-select_module \
--with-http_v2_module \
--with-http_realip_module \
--with-http_addition_module \
--with-http_sub_module \
--with-http_dav_module \
--with-http_stub_status_module \
--with-http_flv_module \
--with-http_mp4_module \
--with-http_gunzip_module \
--with-http_gzip_static_module \
--with-http_auth_request_module \
--with-http_random_index_module \
--with-http_secure_link_module \
--with-http_slice_module \
--with-mail \
--with-stream \
--with-http_ssl_module \
--with-mail_ssl_module \
--with-stream_ssl_module \
--add-module=objs/lib/nginx-rtmp-module
```
