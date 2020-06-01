---
layout: page
title: VMs
include_in_header: true
---

Try out UTM with these free prebuilt VMs! Your performance may vary depending on your device and the OS. For the best experience, choose an OS with SPICE tools and Sharing features installed. For new users, the Debian images are recommended.

## Android

### [Android 2.2](https://github.com/utmapp/vm-downloads/releases/download/android-x86-2.2/Android-2.2.utm.zip)

| Architecture | i386            |
| Memory       | 512MiB          |
| Disk         | 10GiB           |
| Display      | VGA             |
| SPICE tools  | No              |
| Sharing      | No              |
| Username     | none            |
| Password     | none            |

### [Android 4.4](https://github.com/utmapp/vm-downloads/releases/download/android-x86-4.4/Android-4.4.utm.zip)

| Architecture | i386            |
| Memory       | 1024MiB         |
| Disk         | 10GiB           |
| Display      | VGA             |
| SPICE tools  | No              |
| Sharing      | No              |
| Username     | none            |
| Password     | none            |

### [Android 9.0](https://github.com/utmapp/vm-downloads/releases/download/android-x86-9.0/Android-9.0.utm.zip)

| Architecture | x86_64          |
| Memory       | 1024MiB         |
| Disk         | 10GiB           |
| Display      | VGA             |
| SPICE tools  | No              |
| Sharing      | No              |
| Username     | none            |
| Password     | none            |

## Linux

### [ArchLinux ARM](https://github.com/utmapp/vm-downloads/releases/download/archlinux-arm64/ArchLinuxARM-UTM.zip)

| Architecture | aarch64         |
| Memory       | 2048MiB         |
| Disk         | 10GiB           |
| Display      | Console         |
| SPICE tools  | N/A             |
| Sharing      | No              |
| Username     | `root`          |
| Password     | `root`          |

### [Debian 10.4 (osy's Developer Edition) ARM](https://github.com/utmapp/vm-downloads/releases/download/debian-10.4-osy/Debian-osy-UTM.zip)

| Architecture | aarch64         |
| Memory       | 1024MiB         |
| Disk         | 10GiB           |
| Display      | VGA+Console     |
| SPICE tools  | YES\*           |
| Sharing      | YES             |
| Username     | `root`          |
| Password     | `password`      |
| Username     | `debian`        |
| Password     | `debian`        |

* Custom built from a minimal Linux install
* [i3 Window Manager](https://i3wm.org) with [LightDM](https://wiki.debian.org/LightDM) for maximum performance
* Customized xterm theme
* Working audio, networking, sharing features
* In VGA mode, `/media/share` mounts the share directory at startup
* Alias commands `resize` refreshes resolution of the display and `soundon` enables audio

### [Debian 10.4 (LDXE) ARM](https://github.com/utmapp/vm-downloads/releases/download/debian-10.4-ldxe/Debian-ARM-LXDE-UTM.zip)

| Architecture | aarch64         |
| Memory       | 1024MiB         |
| Disk         | 10GiB           |
| Display      | VGA+Console     |
| SPICE tools  | Yes\*           |
| Sharing      | Yes             |
| Username     | `root`          |
| Password     | `password`      |
| Username     | `debian`        |
| Password     | `debian`        |

### [Debian 10.4 (Xfce) ARM](https://github.com/utmapp/vm-downloads/releases/download/debian-10.4-xfce/Debian-ARM-Xfce-UTM.zip)

| Architecture | aarch64         |
| Memory       | 1024MiB         |
| Disk         | 10GiB           |
| Display      | VGA+Console     |
| SPICE tools  | Yes\*           |
| Sharing      | Yes             |
| Username     | `root`          |
| Password     | `password`      |
| Username     | `debian`        |
| Password     | `debian`        |

\* Due to a [bug](https://bugzilla.redhat.com/show_bug.cgi?id=1290586) auto resolution does not work. Run `xrandr --output Virtual-1 --auto` to resize.

### [Debian 10.4 (Minimal) ARM](https://github.com/utmapp/vm-downloads/releases/download/debian-10.4/Debian-ARM-UTM.zip)

| Architecture | aarch64         |
| Memory       | 1024MiB         |
| Disk         | 10GiB           |
| Display      | Console         |
| SPICE tools  | No              |
| Sharing      | No              |
| Username     | `root`          |
| Password     | `password`      |
| Username     | `debian`        |
| Password     | `debian`        |

### [Ubuntu 14.04](https://github.com/utmapp/vm-downloads/releases/download/ubuntu-14.04/Ubuntu-14.04.utm.zip)

| Architecture | x86_64          |
| Memory       | 512MiB          |
| Disk         | 10GiB           |
| Display      | VGA             |
| SPICE tools  | Yes             |
| Sharing      | No              |
| Username     | `ubuntu`        |
| Password     | `ubuntu`        |

### [Ubuntu 18.04](https://github.com/utmapp/vm-downloads/releases/download/ubuntu-18.04/Ubuntu-18.04.utm.7z)

| Architecture | x86_64          |
| Memory       | 1024MiB         |
| Disk         | 10GiB           |
| Display      | VGA             |
| SPICE tools  | Yes             |
| Sharing      | Yes             |
| Username     | `ubuntu`        |
| Password     | `ubuntu`        |

## Other

### [ReactOS 0.4.14](https://github.com/utmapp/vm-downloads/releases/download/reactos-0.4.14-RC10/ReactOS.utm.zip)

| Architecture | x86_64          |
| Memory       | 512MiB          |
| Disk         | 10GiB           |
| Display      | VGA             |
| SPICE tools  | No              |
| Sharing      | No              |
| Username     | `Administrator` |
| Password     | none            |
