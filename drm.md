---
title: DRM
layout: page
group: navigation
permalink: /drm/
order: 05
---

Many streaming services are now implementing Digital Right Management (DRM) security to their streams.

On many platforms, we support decoding of these streams using the Inputstream.Adaptive support available as an optional extra with Kodi v18. This means that you **must be running at least Kodi v18** for this to work.

We have built a `DRM Helper` add-on which manages the installation of the specific libraries required for decoding Widevine encrypted streams through Inputstream.Adaptive.

For this to work, we rely on the Widevine DRM library shipped with the Google Chrome browser, and a layer that translates between it and Inputstream.Adaptive.

For platform support, this means that we can support:

 * Windows (not from Windows Store, see below)
 * Mac OS X
 * Android and Android TV devices (only with included DRM support, see below)
 * Linux x64 and x32
 * Linux ARM v6 and v7 (e.g. Raspberry Pi)

Some platforms that are not supported are:

 * Windows (from Windows Store)
 * Xbox One
 * Android and Android TV devices (mostly Cheap Chinese boxes, see below)

### Windows

For Windows, Kodi can be be installed either directly, or from the Windows Store. When installed from the Windows Store, Kodi is subject to tighter security, which prevents us from being able to load the extra Widevine DRM library. Therefore, we recommend only installing Kodi by downloading it from Kodi directly and running the installer yourself.

### Xbox One

Kodi on the Xbox One is subject to the same security restrictions as Kodi installed on Windows from the Windows Store, where we are unable to load the Widevine DRM library. There is no away around this limitation, so we are unable to provide any Widevine DRM support to the Xbox One.

### Android / Android TV

Android can be supported by native Widevine support that is included within the Android operating system itself, but does require an _official_ device that includes the Widevine support from Google. This generally includes handsets TV boxes TVs from brand-name manufacturers.

This generally means that many cheap Android _sticks_ from China won't include this support.

Devices that we have had great success with, and recommend are:
 * NVIDIA Shield TV
 * Mi Box 3
 * Nexus Player
 * Sony Bravia TVs, powered by Android TV

## Installation

The `DRM Helper` add-on is installed automatically when installing any of our add-ons that require it.

Once you attempt to load up a stream that requires DRM support, you will be prompted to download the required binaries to make this work.
