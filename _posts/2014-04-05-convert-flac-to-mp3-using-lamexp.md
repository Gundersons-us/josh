---
id: 1340
title: convert FLAC to MP3 using LameXP
date: 2014-04-05T01:39:13-07:00
author: joshg253
layout: post
guid: http://blog.gundersons.us/?p=1340
permalink: /2014/04/05/convert-flac-to-mp3-using-lamexp/
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";b:0;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - how-to
  - software
---
I have EAC set up to rip Perfect FLA rips, and then to transcode to MP3 I use an open-source program called LameXP.

<h1>Setup</h1>

Grab the latest LameXP: http://lamexp.sourceforge.net/
Extract the ZIP to a folder, or run the installer
Agree to
Check for updates or Postpone
click Don't Show Again at the Nero AAC

<h2>Disable sounds</h2>

Tools -&gt; Configuration -&gt; Disable Sound Effects
You're welcome. :)

<h2>Output Directory tab</h2>

check "Save output files to the same location where the input file is located"

<h2>Meta Data tab</h2>

double-click Position, change to Unspecified (copy from source file)
double-click Comment, clear the field, OK
Note: you will have to clear the Comment field every time you open the program, unless you want the Comment field in your MP3s to say "Encoded with LameXP". I prefer them to use whatever was in the FLAC.

<h2>Compression tab</h2>

MP3, VBR, Maximum quality
Gives you "V0" MP3s

<h2>Advanced Options tab</h2>

LAME Algorithm Quality all the way to the right (Better quality)
Multi-Threading
The default/recommended setting is "Choose the number of threads based on the number of processors", but the behavior is a little funky:
My laptop has a i5-3210M, with 4 logical processors. LameXP chooses 4 Instances. Makes sense.
My main PC has an i7-970, with 12 logical processors. LameXP chooses 7. WTF?