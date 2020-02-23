---
layout: page
title: FAQ
include_in_header: true
---

## What is this?

UTM is an app for running other operating systems on your iPhone or iPad. It is **not** for running iOS on other systems. This allows you, among other things, to run Windows or Linux on your iOS device at a usable speed.

## Where can I download UTM?

This project is still under development and there is no plan for a release anytime soon. Check out the [Github](https://github.com/utmapp/UTM) for development and build information.

## Does this require a jailbreak?

Currently, UTM does not require a jailbreak to use. It works on iOS 11 and above. However, it is possible that Apple changes the private APIs in the future and break compatibility with non-jailbroken devices. And because of the use of private APIs and the fact that Apple explicitly prohibits JIT code, it is unlikely that UTM will ever be in the App Store and will only be able to run through sideloading (restrictions are discussed below).

Another thing is that in order to comply with the W^X restrictions in the iOS kernel, TCG can only run at about 70% of the speed it would run without the changes. However, that is still fast enough to be usable in many cases, especially in console-only or low-graphics use cases. Potentially in the future, we might maintain a jailbreak app that can run at full speed.

## How do I sideload an app?

Sideloading allows you to load unofficial apps on your iOS device. If you have a free Apple account, you must re-sign the app every 7 days. If you have a paid ($99/year) Apple developer account, you must re-sign the app every year. For more information and other options, search for "ios sideloading" and you can find resources online.

## How does UTM work?

The majority of the work is done by [qemu](https://www.qemu.org). Because iOS devices lack hardware virtualization support, we cannot use the KVM accelerator and instead use the TCG accelerator which does dynamic code translation and JIT compilation. UTM also includes a [SPICE](https://www.spice-space.org) client written for Metal. This connects with the SPICE server in qemu and allows for some para-virtualization as the QXL graphics driver running on the guest OS can send low-level draw commands directly to Metal APIs.

For more in-depth information on the changes made to qemu for JIT to work on iOS, check out [this document](https://github.com/utmapp/qemu/blob/ios-support/docs/devel/ios.rst). 

## What are the limitations?

Currently, the back-end (qemu) is mostly working. It works as well as qemu on macOS, which means that most things boot and devices including user-mode networking and graphics run fine. However, the front-end (the iOS UI) is developed from scratch and is fairly buggy/incomplete. This is where we need the most help currently. Other major things not working includes: ability to start multiple VMs in one session, snapshots, better input controls, and sound.

## How can I contribute?

We need all the help we can get! We need both people to work on improving/optimizing the qemu backend as well as people working on the UI and front-end. You can check out our [Github](https://github.com/utmapp/) and join our [Discord](https://discord.gg/UV2RUgD).
