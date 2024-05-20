# TWRP Device Tree for Xiaomi Redmi S2 (ysl).

## Setup repo tool
Setup repo tool from here https://source.android.com/setup/develop#installing-repo

## Compile

Sync TWRP manifest:

```
repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-12.1
```

Sync the sources with

```
repo sync -j$(nproc --all)
```

To build, execute this command:

```
. build/envsetup.sh; lunch twrp_ysl-eng; make recoveryimage -j$(nproc --all)
```
