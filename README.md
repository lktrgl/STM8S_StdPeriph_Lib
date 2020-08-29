# STM8S_StdPeriph_Lib

Applied SDCC compatibility patch

URL: https://github.com/hbendalibraham/stm8_started

( https://github.com/hbendalibraham/stm8_started/tree/master/STM8_helloworld/STM8S_StdPeriph_Driver )

How to start:

```
git clone  --recurse-submodules --verbose --remote --progress https://github.com/lktrgl/STM8S_StdPeriph_Lib.git \
  && cd STM8S_StdPeriph_Lib/Project/STM8S_StdPeriph_Template/SDCC_CMAKE \
  && mkdir build \
  && cd build \
  && cmake -DCMAKE_TOOLCHAIN_FILE=../Toolchain-sdcc.cmake .. \
  && make all
```

