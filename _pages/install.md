---
layout: page
title: Install
include_in_header: true
---

**If you are running iOS 11, 12, or 13**: UTM does not require a jailbreak to use, but you must sideload it. If you are new to sideloading, it is a way to use a developer's certificate to load unapproved apps on a non-jailbroken iOS device. There are a few limitations to sideloading:

* Free developer accounts must re-sign every 7 days
* Paid developer accounts must re-sign every 1 year

**If you are running iOS 14**: UTM requires(\*) a jailbreak to use. Follow the manual install instructions. (\* You can also run UTM without a jailbreak by [running it tethered to Xcode][6]. However, that is not really convenient.)

## AltStore

The recommended way is to use [AltStore][4] which manages re-signing automatically.

### AltStore Repository

Note: at this time, 3rd party repos require a beta of AltStore which is available only to the developer's Patreon supporters. When installing from the repository, you can recieve update prompts from AltStore.

1. Install [AltStore][4]
2. Add the source: [https://alt.getutm.app][5]
3. Download UTM from AltStore

### AltStore Sideloading

For non beta-testers, the public release of AltStore lacks the ability to add repositories and check updates but can still manage re-signing automatically.

1. Install [AltStore][4]
2. Download the [latest IPA release][1] on your device
3. Open the IPA with AltStore

## Manual Install

[You can download the latest unsigned IPA release from Github.][1]

If you are jailbroken, you can install the unsigned IPA directly with Filza. You should _not_ re-sign it.

If you are running stock iOS, a free and easy way to re-sign an IPA is with [iOS App Signer][2]. Then you can install it with iTunes, Music app, or Xcode.

There are many "cloud" signing services including AppCake that do **not** work with UTM because they use the wrong kind of signing certificate. If you get a crash or a black screen while trying to start a VM, it is likely that your signing certificate was invalid.

You can check if you have the right signing certificate by going to `Settings -> General -> Profiles & Device Management`. If the certificate used for signing UTM is listed under `Developer App`, then it is good. If it is listed under anything else such as `Enterprise App`, then it is the wrong certificate.

## Help and Support

Please [join our Discord][3] for help and support.

  [1]: https://github.com/utmapp/UTM/releases/latest
  [2]: https://dantheman827.github.io/ios-app-signer/
  [3]: https://discord.gg/UV2RUgD
  [4]: https://altstore.io
  [5]: altstore://source?url=https://alt.getutm.app
  [6]: https://github.com/utmapp/UTM/blob/master/Documentation/TetheredLaunch.md
