# Samsung Galaxy A80 (R1Q) TWRP Device Tree

This tree is now moved to official TWRP github available [here](https://github.com/TeamWin/android_device_samsung_r1q).
Latest images are on the [offical TWRP website](https://github.com/TeamWin/android_device_samsung_r1q) as well.

## Building

This device tree is built using TWRP's minimal manifests, which are available [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni).

1. Set up the build environment according to [these instuructions](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni/blob/twrp-9.0/README.md#getting-started).
2. Clone this device tree: 
```bash
git clone -b omni-9.0 https://github.com/Am80286/twrp_samsung_r1q.git device/samsung/r1q
```
3. Start the build: 
```bash
source build/envsetup.sh
lunch omni_r1q-eng
mka recoveryimage
```

After the build is finished, the recovery image is going to be in `out/target/product/r1q/recovery.img `
