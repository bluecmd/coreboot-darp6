# coreboot-darp6

Build:

```
$ export GO111MODULE=off
$ make KERNEL_MAKE_FLAGS='-j8' CPU=$(nproc)
```

Note: Currently coreboot does not handle 1920x1080 resolution since
1080 is not divisible by 16 - so the bootsplash does not work.

The `*.rom` files are taken from https://github.com/system76/firmware-open
