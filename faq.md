---
title: FAQ
layout: page
group: navigation
permalink: /faq/
order: 04
---

#### Repository installation fails with `"Failed to install Add-on from zip file. Installing the Add-on from the zip file located at _path_ failed due to an invalid structure."`
This is due to downloading the wrong repository ZIP file, probably from GitHub's big green download button. Please follow the [installation instructions](/installation/) for the correct ZIP file.  

&nbsp;  
  
#### Add-on installation fails with `failed to install a dependency` error
The `failed to install a dependency` error is caused by Kodi being unable to install a dependency required by our add-ons. The issue is usually due to other third party repositories set up in Kodi which are conflicting with Aussie Add-on's add-ons. Try disabling or removing any repositories such as TVAddons, SuperRepo, Ares and any others you don't specifically require.

&nbsp;

#### DRM streams silenty fail to play with `InputStream Adaptive: Could not open / parse mpdURL` in Kodi's log file
This is due to the `ssd_wv` library missing or an error with it, like a version mismatch between it and the inputstream.adaptive library. You could try re-installing the DRM libraries (from the add-on configuration settings).  

&nbsp;  

#### DRM streams show grey/black screen of garbage with Kodi v17 on Android
The simplest solution for this is to upgrade to a nightly build of Kodi v18 from <a href="http://mirrors.kodi.tv/nightlies/android/">http://mirrors.kodi.tv/nightlies/android/</a>. 

&nbsp;
