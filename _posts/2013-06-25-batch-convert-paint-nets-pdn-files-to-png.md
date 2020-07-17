---
id: 1308
title: batch convert PDN images to PNG
date: 2013-06-25T15:46:37-07:00
author: joshg253
layout: post
guid: http://joshgunderson.info/wp/?p=6
permalink: /2013/06/25/batch-convert-paint-nets-pdn-files-to-png/
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";b:0;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - how-to
tags:
  - Paint.NET
  - Windows
---
<ol>
    <li>Grab <a href="https://www.comsquare.dnsalias.com/forums/viewforum.php?f=23">pdn2png</a></li>
    <li>Drop the exe from the zip into a folder with all your .PDNs</li>
    <li>Open a command window, navigate to said folder, and run:</li>
</ol>

<pre>forfiles /m *.pdn /c "cmd /c pdn2png @file"</pre>

Different command-line switches can be used to change output options, but this worked for me to quickly convert a folder of 128 2-layer PDNs to PNGs.