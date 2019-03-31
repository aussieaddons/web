---
id: afl
title: AFL Video
layout: addon
description: Watch the latest AFL replays, news and match reports. Live streaming and match replays available with a valid AFL Live Pass.
github_url: https://github.com/aussieaddons/plugin.video.afl-video
---

## Current status

AFL Video is fully supported, with the following functionality:

 - Live matches (AFL Live Pass required)
 - Match replays (AFL Live Pass required)
 - On-demand video clips (Coach press-conferences, highlights, Team video, etc)

<div class="bs-callout bs-callout-danger">
  <h4>Kodi version requirement</h4>
  You will need to use at least Kodi v17 for this to function correctly, due to the
  HTTPS encryption enforced on the streaming servers.

  Kodi v18 is required for watching live matches, along with DRM support for
  your platform. See our <a href="/drm">DRM support page</a> for more
  information.
</div>


## Live streaming and match replays

You can use a valid AFL Live Pass subscription to watch live streaming and match
replays through this add-on. This can be either a subscription paid for through AFL.com.au
or it can be a Telstra free subscription through a mobile plan.

<div class="bs-callout bs-callout-danger">
  <h4>DRM support required for live matches</h4>
  Since the 2019 season, live AFL matches are now protected with DRM.

  Kodi v18 is required for watching live matches, along with DRM support for
  your platform. See our <a href="/drm">DRM support page</a> for more
  information.
</div>

To sign on, it is recommended you install the AFL app to your Android or iOS device
and follow the setup instructions. Once completed, you should enter your account details
into the AFL Video add-on settings.

Live streaming is intended for mobile use only, and so the quality is poor, but watchable.


## Live Pass Subscriptions
There are 3 ways to obtain an AFL Live Pass in 2018:

1. Purchase a weekly/monthly/yearly subscription directly from the afl.com.au website
2. Purchase a weekly/monthly/yearly subscription as an _in-app_ purchase from the
AFL app on your mobile/tablet device,
whether it be from Google Play or Apple's App Store
3. Receive a free subscription as an eligible Telstra customer as long as you continue to meet the requirements (post-paid mobile plan, $30+ pre-paid recharge)

### Method 1: afl.com.au website subscription
You can sign up for a Live Pass weekly/monthly/yearly subscription directly through https://subscription.afl.com.au/.

The AFL use Telstra ID, so you can use an existing Telstra ID, or create a new one.

Simply enable the **Live Pass Subscription** setting in the add-ons settings,
choose *Paid (afl.com.au)* as the subscription type and enter your Telstra ID
username and password.

### Method 2: In-app purchase
There is no easy way for us to retrieve the credentials required to have the Kodi add-on _log in_ using any sort of username and password.
Luckily though the AFL app will actually display our login token for us, all we have to do is enter it in the Kodi add-on settings.
Instructions are handily available from the Kodi add-on settings itself and here.

Open the AFL app on your device and obtain your Live Pass subscription.
Once logged in the purple T at the top right of the home screen should turn green.

Press on the green T which will open the settings, and go into _AFL Live Pass Subscription_.
Scroll to the bottom of the screen to find the mis-uuid token.

Open the add-on settings, enable the **Live Pass Subscription** setting and select **Paid (in-app purchase)** as your subscription type.

Then enter the 32 digit hexadecimal number that comes after **mis-uuid-** into the subscription token setting.

It's not going to be much fun entering this in if you're using a TV remote control.

If you have access to anything else like a USB keyboard or smartphone remote control for Kodi then definitely save yourself the frustration.


### Methods 3: Telstra free subscription
Telstra customers with a post-paid or pre-paid ($30 minimum recharge) mobile service are eligible for a free Live Pass.

The AFL app can detect your service details through the mobile network, but for Kodi, we need to specifically
link your subscription with a Telstra ID username and password.

Please use [http://hub.telstra.com.au/sp2017-afl-app](http://hub.telstra.com.au/sp2017-afl-app) to either
register a new Telstra ID or use an existing one to confirm that your Telstra ID has an eligible service attached.

Then, open the add-on settings, enable the **Live Pass Subscription** setting and
select **Free offer (Telstra ID)** as your subscription type.

There are a few exceptions to Telstra's system that are incompatible with the free Live Pass offer.
Home broadband customers and any Telstra IDs that are linked to home broadband accounts are incompatible/ineligible.
There may also be other service types that cause this issue.

The work around is simply to create a new Telstra ID and re link your eligible service to that.
