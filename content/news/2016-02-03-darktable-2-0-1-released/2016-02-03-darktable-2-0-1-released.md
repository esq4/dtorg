author: houz
comments: true
date: 2016-02-03 20:45:27+00:00
layout: post
link: http://www.darktable.org/2016/02/darktable-2-0-1-released/
slug: darktable-2-0-1-released
title: darktable 2.0.1 released
lede: race_cars_wide.jpg
lede_author: <a href="https://houz.org/">houz</a>
wordpress_id: 3945
tags: announcement, darktable release

we're proud to announce the first bugfix release for the 2.0 series of darktable, 2.0.1!

the github release is here: [https://github.com/darktable-org/darktable/releases/tag/release-2.0.1](https://github.com/darktable-org/darktable/releases/tag/release-2.0.1)

as always, please don't use the autogenerated tarball provided by github, but only our tar.xz. the checksums are:

    $ sha256sum darktable-2.0.1.tar.xz
    4d0e76eb42b95418ab59c17bff8aac660f5348b082aabfb3113607c67e87830b  darktable-2.0.1.tar.xz
    $ sha256sum darktable-2.0.1.dmg
    580d1feb356e05d206eb74d7c134f0ffca4202943388147385c5b8466fc1eada  darktable-2.0.1.dmg

and the changelog as compared to 2.0.0 can be found below.

## New features:

* add export variables for Creator, Publisher and Rights from metadata
* add support for key accels for spot removal iop
* add some more info to `--version`
* add collection sorting by group_id to keep grouped images together
* add `$(IMAGE.BASENAME)` to watermark
* OSX packaging: add darktable-cltest
* OSX packaging: add darktable-generate-cache

## Bugfixes:

* make sure GTK prefers our CSS over system's
* make selected label's background color visible
* make ctrl-t completion popup nicer
* fixed folder list scrolling to the top on select
* scale waveform histogram to hidpi screens
* really hide all panels in slideshow
* add filename to missing white balance message
* fix wrong tooltip in print scale
* changing mask no longer invalidates the filmstrip thumb, making it faster
* fix calculated image count in a collection
* don't allow too small sidepanels
* fixes white balance sliders for some cameras
* fix some memleaks
* code hardening in color reconstruction
* validate noiseprofiles.json on startup
* no longer lose old export presets
* fix some crash with wrong history_end
* don't load images from cameras with CYGM/RGBE CFA for now
* some fixes in demosaicing
* fix red/blue interpolation for XTrans
* fix profiled denoise on OpenCL
* use sRGB when output/softproof profile is missing
* fix loading of .hdr files
* default to libsecret instead of gnome keyring which is no longer supported
* fix a bug in mask border self intersections
* don't allow empty strings as mask shape names
* fix a crash in masks
* fix an OpenCL crash
* eliminate deprecated OpenCL compiler options
* update appdata file to version 0.6
* allow finding Saxon on Fedora 23

## Camera support:

* Fujifilm XQ2 raw support
* support all Panasonic FZ150 crop modes
* basic support for Nikon 1 V3
* add defs for Canon CHDK DNG cameras to make noise profiles work

## White balance presets:

* add Nikon D5500
* add Nikon 1 V3
* add missing Nikon D810 presets
* add Fuji X100T

## Basecurves:

* copy X100S to X100T

## Noise profiles:

* fix typo in D5200 profiles to make them work again
* add Panasonic FZ1000
* add Nikon D5500
* add Ricoh GR
* add Nikon 1 V3
* add Canon PowerShot S100
* copy Fuji X100S to X100T

## Translations:

* add Hungarian
* update German
* update Swedish
* update Slovak
* update Spanish
* update Dutch
* update French