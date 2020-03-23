---
layout: page
title: Install
include_in_header: true
---

UTM does not require a jailbreak to use, but you must sideload it. If you are new to sideloading, it is a way to use a developer's certificate to load unapproved apps on a non-jailbroken iOS device. There are a few limitations to sideloading:

* Free developer accounts must re-sign every 7 days
* Paid developer accounts must re-sign every 1 year
* iOS 13.3.1 has a signing bug with free accounts, you can use any lower or higher iOS version

## Download

[You can download the latest unsigned IPA release from Github.][1]

## Signing

If you are jailbroken, you can install the unsigned IPA directly with Filza. You should _not_ re-sign it.

If you are running stock iOS, a free and easy way to re-sign an IPA is with [iOS App Signer][2]. Then you can install it with iTunes, Music app, or Xcode.

There are many "cloud" signing services including AppCake that do **not** work with UTM because they use the wrong kind of signing certificate. If you get a crash while trying to start a VM, it is likely that your signing certificate was invalid.

You can check if you have the right signing certificate by going to `Settings -> General -> Profiles & Device Management`. If the certificate used for signing UTM is listed under `Developer App`, then it is good. If it is listed under anything else such as `Enterprise App`, then it is the wrong certificate.

## Help and Support

Please [join our Discord][3] for help and support.

  [1]: https://github.com/utmapp/UTM/releases/latest
  [2]: https://dantheman827.github.io/ios-app-signer/
  [3]: https://discord.gg/UV2RUgD
