---
layout: post
title: 'ZoneMinder Release 1.36.0: The Memory Remains'
author: Isaac Connor
---

## Thank You to Those who have Contributed
We continue to thank those that have contributed to the ZoneMinder project. ZoneMinder is a community based FOSS project. As such, we are constantly in need of those willing to volunteer their time to maintain and improve it, whether that be writing code, answering questions in the forum, or updating our documentation. Please consider helping us

Also a special thank you to those who contribute monetarily. Without your donations the devs would have less time to devote to ZoneMinder.

## We DO NOT RECOMMEND running any prior version of ZoneMinder

## Major Release 1.36.0

## Changes since 1.34.*

# Filters
- Moved event email options from global config to per Filter
- Added user to run filter as, so that users without access to certain monitors can't just use a filter to access them.
- Filters now have PreSQL and PostSQL conditions. The first Post SQL condition is ExistsInFileSystem. This can be used to cleanup after a crash instead of using zmaudit.
- Warnings on Filter edit page when you create a filter than can delete archived events.
- Added Auto Unarchive function

# UI Updates
- Bootstrap updated to version 3
- Removed mootools
- Events list now uses bootstrap-table to enable a more modern powerful ui
- Scaled thumbnail on mouseover on events list
- Thumbnails with scaling on console
- Frames view updates to include stats information
- Many popups turned into modals
- Monitor edit is now a full view instead of popup
- Zone edit is now scaled so high res cameras don't take the entire screen or more.
- Added Estimated RAM use to Buffers tab in Monitors.
- Monitor edit no longer form submits/reloads between tabs it just hides/unhides tabs using bootstrap nav.
- Monitors can now have Latitude/Longitude associated and displayed on a map

# General
- New Monitor type VNC for recording desktops
- Better use of scaling when streaming to reduce bandwidth/cpu use
- Dynamic loading of vlc, curl and other libraries that might not be used. Saves ram
- ONVIF probe can now select a network to scan
- Sessions now stored in database
- Event Summary tables reorganized to improve locking performance
- Clicking on username in header will now list other logged in users if you have SystemView permission.
- ZoneMinder will now try other Storage Areas if it can't create the event in the assigned area.
- New Monitor Setting: Decoding Enabled/Disabled
- /dev/shm mmap use decoupled from image buffering. You should set ImageBufferCount to 3 or larger.
- Mp4v2 deprecated and removed.
- Zma process has been turned into a thread of zmc.
- Added second ffmpeg input stream for when audio is coming from another source.
- Added RTSP re-streaming
- Hwaccel encoding support for intel vaapi and nvenc
- Use onmousedown/onmouseup for PTZ start/stop in PTZ controls. Amcrest is the only Protocol that supports it so far.

To update to this release on Ubuntu, you will need to add the new ppa
sudo add-apt-repository ppa:iconnor/zoneminder-1.36

# Change Log

## [1.36.0](https://github.com/ZoneMinder/zoneminder/tree/1.36.0) (2021-05-14)
[Full Changelog](https://github.com/ZoneMinder/zoneminder/compare/1.34.0...1.36.0)

