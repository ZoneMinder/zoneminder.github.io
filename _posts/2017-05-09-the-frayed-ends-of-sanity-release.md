---
layout: post
title: 'ZoneMinder Release 1.30.4: The Frayed Ends of Sanity'
author: Andrew Bauer
---

## Small Fix

This release has been created to address an issue which was discovered in the new uridecode function. There are some minor packaging related changes made as well.  What follows has been copied and pasted from the previous release notes to make sure everyone reads it.

## Cake PHP API Note
The previous 1.30.2 release disabled cake php debug mode due to a potential security vulnerability. Be advised that, because cake debug mode is off, the cake debug web page, typically navigated to with a /zm/api suffix, is also turned off. The API itself will continue to function normally.

## Important Note to Package Maintainers
Switching to the php apc cache engine adds a new package dependency on the php-apc or php-apcu package. The exact name of the package varies per distro. The API will not function without this package installed and the web server restarted.

## Nightly Builds
We have recently enabled a nightly build system, which is cranking out rpm & deb packages almost as fast as we make changes to the source code.  If you have an interest in testing a recent build of the master branch then this is for you. This will allow you to test bleeding edge software changes w/o having to first be an expert in building rpm or deb packages. Nightly build rpm packages are currently available at [zmrepo.zoneminder.com](https://zmrepo.zoneminder.com). As soon as I learn where Isaac is hosting the deb packages, I will update these release notes.

## Thank You to Those who have Contributed
We continue to thank those that have contributed to the ZoneMinder project. We are always in need of volunteers, not just to write code, but to help manage the user forum, manage wiki content, write documentation, test the latest master branch, etc. There is always far more work to do than people available to do the work.

What follows is the complete change log since our previous release:

# Change Log

## [1.30.4](https://github.com/ZoneMinder/ZoneMinder/tree/1.30.4) (2017-05-09)
[Full Changelog](https://github.com/ZoneMinder/ZoneMinder/compare/1.30.3...1.30.4)

**Merged pull requests:**

- update ubuntu builds with dependencies on php-apcu and php-apc and php-apcu-bc [\#1873](https://github.com/ZoneMinder/ZoneMinder/pull/1873) ([connortechnology](https://github.com/connortechnology))
- fix uridecode\(password\) to uridecode\(value\) [\#1872](https://github.com/ZoneMinder/ZoneMinder/pull/1872) ([connortechnology](https://github.com/connortechnology))
- Clean up ubuntu builds [\#1871](https://github.com/ZoneMinder/ZoneMinder/pull/1871) ([connortechnology](https://github.com/connortechnology))
