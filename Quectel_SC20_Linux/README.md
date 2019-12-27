# Get the code source
``` shell
git clone ssh://git@gitlab.quectel.com:2222/quectel_smart/sc20_linux.git
```

# Docker image for build quectel_sc20_linux
``` shell
docker build . -t arcayi/quectel_sc20_linux
```

```shell 
cd poky
source build/conf/set_bb_env.sh
build-8909-quec-smart-image
```

# Known issues
