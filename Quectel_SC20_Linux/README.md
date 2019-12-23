# Docker image for build quectel_sc20_linux
docker build . -t arcayi/quectel_sc20_linux

# Known issues

* Do not use Bitbake as root.

``` bash
touch /build/poky/build/conf/sanity.conf
```
