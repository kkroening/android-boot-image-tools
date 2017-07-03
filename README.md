# Android Boot Image Tools

Packing/repacking Android boot images is annoying.  `Android Boot Image Tools` makes it a breeze.

## Dependencies

Make sure `cpio`, `mkbootimg`, and `unmkbootimg` are on your `$PATH`.

`cpio` seems to be fairly standard and shouldn't require special installation.
`mkbootimg`/`unmkbootimg` can be found here: https://github.com/pbatard/bootimg-tools

## Usage

### Extract kernel file from boot.img:

```
abit get-kernel boot.img kernel
```

### Extract ramdisk directory from boot.img:

```
abit get-ramdisk boot.img ramdisk
```

### Insert kernel file into boot.img:

```
abit put-kernel boot.img kernel [-o boot2.img]
```

### Insert ramdisk dir into boot.img:

```
abit put-ramdisk boot.img ramdisk [-o boot2.img]
```
