# TWRP Tree for Xiaomi Mi Note 3
```
#
# Copyright (C) 2012-2024 Team Win Recovery Project
#
# SPDX-License-Identifier: Apache-2.0
#
```

## Device specifications

|                  Device | Xiaomi Mi Note 3                                                         |
|------------------------:|--------------------------------------------------------------------------|
|                     SoC | Qualcomm SDM660 Snapdragon 660                                           |
|                     CPU | Quad-core 2.2GHz Kryo 260 & quad-core 1.8GHz Kryo 260                    |
|                     GPU | 850MHz Adreno 512                                                        |
|                  Memory | 6 GB RAM (LPDDR4 1866MHz dual-channel)                                   |
| Shipped Android version | 7.1                                                                      |
|                 Storage | 64 GB (eMMC 5.1 Flash)                                                   |
|                 Battery | Non-removable Li-Po 3500 mAh                                             |
|              Dimensions | 152.6 x 73.95 x 7.6 mm                                                   |
|                 Display | 1920 x 1080 px, 5.5 inches (403 PPI)                                     |
|             Rear camera | Dual 12 MP, f/2.0, phase detection autofocus, dual-LED (dual tone) flash |
|            Front camera | 16 MP, 2.0 µm pixel size                                                 |

![Xiaomi Mi Note 3](https://i1.mifile.cn/f/i/17/minote3/specs_black.jpg "Xiaomi Mi Note 3 in black")

## Compile

First repo init the TWRP 12.1 tree:

```shell
repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-12.1
```

Sync source:

```shell
repo sync
```

Finally execute these:

```
.build/envsetup.sh
lunch twrp_jason-eng
mka recoveryimage
```
