---
layout: page
title: FAQ
include_in_header: true
---

## What is this?

UTM is an app for running other operating systems on your iPhone or iPad. It is **not** for running iOS on other systems. This allows you, among other things, to run Windows or Linux on your iOS device at a usable speed.

## Does this require a jailbreak?

Currently, UTM does not require a jailbreak to use. It works on iOS 11 and above. However, it is possible that Apple changes the private APIs in the future and break compatibility with non-jailbroken devices. And because of the use of private APIs and the fact that Apple explicitly prohibits JIT code, it is unlikely that UTM will ever be in the App Store and will only be able to run through sideloading (restrictions are discussed below).

## How do I sideload an app?

Sideloading allows you to load unofficial apps on your iOS device. If you have a free Apple account, you must re-sign the app every 7 days. If you have a paid ($99/year) Apple developer account, you must re-sign the app every year. For more information checkout the [install page]({% link _pages/install.md %}).

## How does UTM work?

The majority of the work is done by [qemu](https://www.qemu.org). Because iOS devices lack hardware virtualization support, we cannot use the KVM accelerator and instead use the TCG accelerator which does dynamic code translation and JIT compilation. UTM also includes a [SPICE](https://www.spice-space.org) client written for Metal. This connects with the SPICE server in qemu and allows for some para-virtualization as the QXL graphics driver running on the guest OS can send low-level draw commands directly to Metal APIs.

For more in-depth information on the changes made to qemu for JIT to work on iOS, check out [this document](https://github.com/utmapp/qemu/blob/ios-support/docs/devel/ios.rst). 

## What are the limitations?

The lack of hardware virtualization on Apple A-chips means that even for ARM code we must re-compile it with JIT. Therefore performance would never reach the levels possible with KVM. There is also no support for GPU virtualization so that means no DirectX or OpenGL. This makes most modern games non-playable.

## How can I contribute?

We need all the help we can get! We need both people to work on improving/optimizing the qemu backend as well as people working on the UI and front-end. You can check out our [Github](https://github.com/utmapp/) and join our [Discord](https://discord.gg/UV2RUgD).
