---
title: DRM
layout: page
group: navigation
permalink: /drm/
order: 05
---

Many streaming services are now implementing Digital Right Management (DRM) security to their streams.

On many platforms, we support decoding of these streams using the Inputstream.Adaptive support available as an optional extra with Kodi v18. This means that you **must be running at least Kodi v18** for this to work.

<div class="bs-callout bs-callout-danger">
  <h4>Kodi version requirement</h4>
  DRM support is available only in Kodi v18 (or newer) through the
  Inputstream.Adaptive add-on, which may need be installed for your platform.
</div>

We have built a `DRM Helper` add-on which manages the installation of the specific libraries required for decoding Widevine encrypted streams through Inputstream.Adaptive.

For this to work, we rely on the Widevine DRM library shipped with the Google Chrome browser, and a layer that translates between it and Inputstream.Adaptive. This means we can generally support any platform that Google Chrome is built for.

## Supported platforms

The platforms that we can support are:

 * Windows (not UWP from Windows Store, see below)
 * Mac OS X
 * Android and Android TV devices (only with included DRM support, see below)
 * Linux x64 and x32
 * Linux ARMv7 and ARMv8 (e.g. Raspberry Pi 2/3)

## Unsupported platforms

Some specific platforms that we can't support (for various reasons):

 * Windows (UWP, from Windows Store)
 * Xbox One
 * iOS (including Apple TV)
 * Android and Android TV devices (mostly Cheap Chinese boxes, see below)
 * Linux ARMv6 (e.g. Raspberry Pi 1)

## Specific platform details

### Windows

For Windows, Kodi can be be installed either directly, or from the Windows Store. When installed from the Windows Store, Kodi is subject to tighter security, which prevents us from being able to load the extra Widevine DRM library. Therefore, we recommend only installing Kodi by downloading it from Kodi directly and running the installer yourself.

### Xbox One

Kodi on the Xbox One is subject to the same security restrictions as Kodi installed on Windows from the Windows Store, where we are unable to load the Widevine DRM library. There is no away around this limitation, so we are unable to provide any Widevine DRM support to the Xbox One.

### Android and Android TV

Android can be supported by native Widevine support that is included within the Android operating system itself, but does require an _official_ device that includes the Widevine support from Google. This generally includes handsets TV boxes TVs from brand-name manufacturers.

This generally means that many cheap Android devices from China won't include this support, or support is broken. In some cases, using a third party firmware can break DRM decoding support. 

Devices that we have had great success with, and recommend are:
 * NVIDIA Shield TV
 * Mi Box 3
 * Nexus Player
 * Sony Bravia TVs, powered by Android TV

## Installation

The `DRM Helper` add-on is installed automatically when installing any of our add-ons that require it.

Once you attempt to load up a stream that requires DRM support, you will be prompted to download the required binaries to make this work.
