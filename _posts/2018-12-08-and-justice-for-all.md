---
layout: post
title: 'ZoneMinder Release 1.32.3: And Justice for All'
author: Andrew Bauer
---

## Thank You to Those who have Contributed
We continue to thank those that have contributed to the ZoneMinder project. ZoneMinder is a community project. As such, we are constantly in need of those willing to volunteer their time to maintain and improve it, whether that be writing code, answering questions in the forum, or updating our documentation. Please consider helping us.

## Bug Fix Release
This is another bug fix release.

Here is a summary of the changes:
- Better support for ZoneMinder behind a (reverse) proxy
- Fix triggers to sum event counts properly
- fix API getVersion call
- fix shared memory alignment errors on some 32bit systems
- fix return user/pass credentials when auth relay is plain

## What's New
If you are upgrading from a release older than 1.32.0, then it is critically important to read the [release notes](https://github.com/ZoneMinder/zoneminder/releases/tag/1.32.0) for the 1.32.0 release. There are several critical changes you should be aware of. Please read them. It is painfully obvious to us who has and has not read the release notes in our user forum.

# Change Log

## [1.32.3](https://github.com/ZoneMinder/zoneminder/tree/1.32.3) (2018-12-08)
[Full Changelog](https://github.com/ZoneMinder/zoneminder/compare/1.32.2...1.32.3)

**Merged pull requests:**

- strip port from HTTP\_HOST [\#2335](https://github.com/ZoneMinder/zoneminder/pull/2335) ([connortechnology](https://github.com/connortechnology))
- Fix rate resetting [\#2329](https://github.com/ZoneMinder/zoneminder/pull/2329) ([connortechnology](https://github.com/connortechnology))
- returns user=&pass= in credentials for auth\_relay plain and none  \#2327 [\#2328](https://github.com/ZoneMinder/zoneminder/pull/2328) ([pliablepixels](https://github.com/pliablepixels))
- Add description for Stream Replay Image Buffer [\#2325](https://github.com/ZoneMinder/zoneminder/pull/2325) ([epruesse](https://github.com/epruesse))
- Fix unreadable input text when OS theme dark [\#2324](https://github.com/ZoneMinder/zoneminder/pull/2324) ([epruesse](https://github.com/epruesse))
- Fix triggers to sum event counts properly [\#2323](https://github.com/ZoneMinder/zoneminder/pull/2323) ([knight-of-ni](https://github.com/knight-of-ni))
- fix \#2317 [\#2322](https://github.com/ZoneMinder/zoneminder/pull/2322) ([connortechnology](https://github.com/connortechnology))
- rpm sub-packages [\#2314](https://github.com/ZoneMinder/zoneminder/pull/2314) ([knight-of-ni](https://github.com/knight-of-ni))
- remove epadding2, to restore the 64bit alignment of startup\_time.   [\#2307](https://github.com/ZoneMinder/zoneminder/pull/2307) ([connortechnology](https://github.com/connortechnology))
- Fix typos in README file [\#2301](https://github.com/ZoneMinder/zoneminder/pull/2301) ([rafidashab](https://github.com/rafidashab))
- Adding "Storage Tag" in definemonitor.rst [\#2299](https://github.com/ZoneMinder/zoneminder/pull/2299) ([aktarus82](https://github.com/aktarus82))
- Use the global dbh in ZoneMinder::Database instead of keeping our own… [\#2298](https://github.com/ZoneMinder/zoneminder/pull/2298) ([connortechnology](https://github.com/connortechnology))
- update nginx support on redhat [\#2293](https://github.com/ZoneMinder/zoneminder/pull/2293) ([knight-of-ni](https://github.com/knight-of-ni))
- updated API - streaming/server/storage/other edits [\#2291](https://github.com/ZoneMinder/zoneminder/pull/2291) ([pliablepixels](https://github.com/pliablepixels))
- Audio only with ffmpeg [\#2289](https://github.com/ZoneMinder/zoneminder/pull/2289) ([connortechnology](https://github.com/connortechnology))
- rough in adding Monitor\_Status to Monitors [\#2288](https://github.com/ZoneMinder/zoneminder/pull/2288) ([connortechnology](https://github.com/connortechnology))
- API - Disable E\_NOTICE from php error reporting in cake debug [\#2286](https://github.com/ZoneMinder/zoneminder/pull/2286) ([ratmole](https://github.com/ratmole))
- Fixes for a couple issues in the Ubuntu guide [\#2285](https://github.com/ZoneMinder/zoneminder/pull/2285) ([chrisk](https://github.com/chrisk))
- Fix 2279 delete camera through api [\#2281](https://github.com/ZoneMinder/zoneminder/pull/2281) ([connortechnology](https://github.com/connortechnology))
- Document /api/monitors/daemonStatus/ [\#2278](https://github.com/ZoneMinder/zoneminder/pull/2278) ([mnoorenberghe](https://github.com/mnoorenberghe))
- use json\_encode/decode instead of serialize/unserialize to pass onvif… [\#2273](https://github.com/ZoneMinder/zoneminder/pull/2273) ([connortechnology](https://github.com/connortechnology))
- API getVersion Fix -\> Undefined variable: eTagMatches... [\#2268](https://github.com/ZoneMinder/zoneminder/pull/2268) ([ratmole](https://github.com/ratmole))
- Bosnian translation [\#2266](https://github.com/ZoneMinder/zoneminder/pull/2266) ([dado-ca](https://github.com/dado-ca))
- Include the remoteAddr in the session authhash cache, so that a chang… [\#2264](https://github.com/ZoneMinder/zoneminder/pull/2264) ([connortechnology](https://github.com/connortechnology))
- show event notes in same event view [\#2259](https://github.com/ZoneMinder/zoneminder/pull/2259) ([pliablepixels](https://github.com/pliablepixels))
- Added monitor preset for D-link DCS-930L [\#2255](https://github.com/ZoneMinder/zoneminder/pull/2255) ([azend](https://github.com/azend))
- Fixed cambozola typo [\#2252](https://github.com/ZoneMinder/zoneminder/pull/2252) ([azend](https://github.com/azend))
- Server path prefix [\#2152](https://github.com/ZoneMinder/zoneminder/pull/2152) ([connortechnology](https://github.com/connortechnology))

\* *This Change Log was automatically generated by [github_changelog_generator](https://github.com/skywinder/Github-Changelog-Generator)*
