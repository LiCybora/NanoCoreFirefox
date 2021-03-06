# Nano Adblocker For Firefox Is No Longer Maintained!

As of upstream [sell the project to unknown developers](https://github.com/NanoAdblocker/NanoCore/issues/362), I refuse to maintain the project for stranger(s) that never show up to introduce themselves to their users.

**NOTE: Unlike upstream, Nano Adblocker on this port is under my control and not related to any upstream's developer(s)!**

For more details or questions, visit [my issue ticket](https://github.com/LiCybora/NanoDefenderFirefox/issues/187). If you can't read English, use a translator or raise your problem on [this issue ticket](https://github.com/LiCybora/NanoDefenderFirefox/issues/187) such that other volunteer can help.

## What Should I Do?!

1. Backup settings: In Nano Adblocker, Go to `Dashboard` > `Settings` > `Backup to files`. (Optional )
2. Backup Filter Lists: Take a screenshot of your Filter List such that you can recover later. (Optional)
3. Disable/Remove Nano Adblocker: In Firefox, Go to `Add-ons` and Disable Nano Adblocker. You may also remove it later if you sure everything are backup and reversible.

## But I Need An Ad-blocker!

Try [uBlock Origin](https://github.com/gorhill/uBlock) where Nano Adblocker forked from. Their interfaces are similar and quite easy to familiar with. [This article](https://github.com/LiCybora/NanoCore2/blob/master/notes/migrate.md) explains the difference between two extensions. **It is recommended to manually restore by copying settings and filters to fresh uBO**. But in case you are too lazy to restore manually, you may still perform:

1. In uBlock Origin, Go to `Dashboard` > `Settings`
2. Click `Restore from file...` and choose the file you backup from previous section.
3. Read [migration note](https://github.com/LiCybora/NanoCore2/blob/master/notes/migrate.md) to watch out incompatibility for avoiding unexpected behavior.

Since uBlock Origin and Nano Adblocker do not share exactly same built-in filter list. In case restore cannot fully recover all filter list, you may manually add back according to the screenshot you take from previous section.

Of course, you are free to choose any ad-blocker you want! Above is just my personal recommendation.

## What If I Really Want to Use Nano Adblocker?

No problem, you can still use it. Filter list can still be updated and you can use it as usual. 

But it is not recommended because you won't receive update anymore. No fix will be released when you experience issue(s). In future, you may not be able to use filter rule that is written in new syntax which is released after the retirement.

## Timeline for Retirement

v1.0.0.154 will be the final version of Nano Adblocker. Extension will be unlisted from AMO one week after released, no more new installation from AMO. You may still install from [my repository](https://github.com/LiCybora/NanoCoreFirefox/releases) after that day if you really want Nano Adblocker back.

It is highly recommended to install alternative instead of continue using Nano Adblocker, however.

## Final Words from Maintainer

Thanks for all volunteer that contribute to this project. Also thanks for users reporting issue to benefit other users as well. Thanks for all users choose Nano Adblocker as their content-blocker.
Hope everyone can still enjoy clean web site in future.

# Nano Adblocker Core for Firefox

Just another adblocker on Firefox

Nano Adblocker is based on [uBlock Origin](https://github.com/gorhill/uBlock).

This repository contains only auto-update script and documentations.

The code of the builder can be found in the [Nano Core 2 repository](https://github.com/LiCybora/NanoCore2). 

The built code can be found in the [release](https://github.com/LiCybora/NanoCoreFirefox/releases).

## Installation

You need Firefox version 55 (57 for Android) or above to install this extension, 
but require 57+ for HTML filtering.

Caution: You need Firefox 60+ for keyboard shortcuts assignment!

### Normal Install

Click .xpi file to download and install from link below.

### [Get it here (for Firefox 55+, including Waterfox)](https://github.com/LiCybora/NanoCoreFirefox/releases/)

### [Get it on AMO (Recommend, Firefox 57+ ONLY)](https://addons.mozilla.org/en-US/firefox/addon/nano-adblocker-firefox/)

**IMPORTANT: DO NOT install both versions.**

### [Get also Nano Defender, the perfect companion extension for Nano Adblocker](https://jspenguin2017.github.io/uBlockProtector)

Note: If you decide to pair with Nano Defender, please install both extensions from same source. 
That is: either both from AMO OR both from GitHub.
Otherwise, you will have to go through Step 2 of [extra installation step](https://jspenguin2017.github.io/uBlockProtector/#extra-installation-steps-for-ublock-origin) (but not other steps).

## Notable Change

### Customizable short keys for Mac Machine (Experimental)

![Screenshot](https://i.imgur.com/If3yfEe.png)

Available since 1.0.0.67

### \[[Work in progress](https://github.com/NanoAdblocker/NanoCore/issues/1)\] Nano Filter Linter, neat and saves frustration

![Screenshot](https://i.imgur.com/SStKkqq.png)

Partially available since 1.0.0.22

### Nano Filter Viewer, powerful and blazing fast

![Screenshot](https://i.imgur.com/fZh4Hqn.png)

Available since 1.0.0.10

### [Nano Extra Resources](https://github.com/NanoAdblocker/NanoFilters/blob/master/NanoFiltersSource/NanoResources.txt), useful and configurable

![Screenshot](https://i.imgur.com/0HIYf4d.png)

Available since 1.0.0.6

### Nano Filter Highlighter, beautiful and helpful

![Screenshot](https://i.imgur.com/KktoFJL.png)

Available since 1.0.0.0

## Other Change

*Note: user interface and other housekeeping changes are not listed here.*

- [Extended advanced settings](https://github.com/NanoAdblocker/NanoCore2/blob/master/notes/advanced_settings.md#advanced-settings)
- [Tweaked filter syntax](https://github.com/NanoAdblocker/NanoCore2/blob/master/notes/filter_syntax.md#filter-syntax)
- Enabled `Block CSP reports` by default (to prevent websites from abusing it
  to track users)
- Added a few more filters to filters manager
- Made cache control button to be always shown
- Added force scroll mode (to be used with element zapper)
