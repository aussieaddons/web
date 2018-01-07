---
title: DRM
layout: page
group: navigation
permalink: /drm/
order: 05
---

Many streaming services are now implementing Digital Right Management (DRM) security to their streams.

On many platforms, we support decoding of these streams using the Inputstream.Adaptive support found in Kodi v17 and later.

We have built a `DRM Helper` add-on which manages the installation of the specific libraries required for decoding Widevine encrypted streams through Inputstream.Adaptive.

For this to work, we rely on the Widevine DRM library shipped with the Google Chrome browser, and a layer that translates between it and Inputstream.Adaptive.

For platform support, this means that we can support:

 * Windows
 * Mac OS X
 * Linux x64 and x32
 * Linux ARM v7 and v8 (32bit) (e.g. Raspberry Pi 2 & 3)

### Android

Android can be supported by native Widevine support that is included within the Android operating system itself, but does require an _official_ device that includes the Widevine support from Google.

This generally means that many cheap Android _sticks_ from China won't include this support.

<div class="bs-callout bs-callout-danger">
  <h4>Issues decoding DRM content with Kodi v17 on Android</h4>
  In some cases, decoding DRM content will fail in Kodi v17 and you will see a grey/black screen of garbage. The simplest solution for this is to upgrade to a nightly build of Kodi v18 from <a href="http://mirrors.kodi.tv/nightlies/android/">http://mirrors.kodi.tv/nightlies/android/</a>
</div>

## Installation

The `DRM Helper` add-on is installed automatically when installing any of our add-ons that require it.

Once you attempt to load up a stream that requires DRM support, you will be prompted to download the required binaries to make this work.
