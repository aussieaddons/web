---
layout: post
title: "DRM decoding issues with Kodi v17 and Android"
description: "DRM can fail to decode streams properly on Android with Kodi v17. Use nightly build of Kodi v18 to fix this."
---

We've seen issues where Plus7 streams encoded with Widevine DRM can fail to
decode properly, and may show a gray or black screen of garbage. This is due
to a library mismatch of the Widevine libraries.

This can be solved by updating the Widevine binaries in the Kodi ARM library
directory, but a simpler solution is to update to a nightly build of Kodi v18
(Leia) until a stable release of Kodi v18 is available in the Google Play
Store.

You can find the nightly builds of Kodi v18 at [http://mirrors.kodi.tv/nightlies/android/](http://mirrors.kodi.tv/nightlies/android/).
