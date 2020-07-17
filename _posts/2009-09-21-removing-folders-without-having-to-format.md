---
id: 694
title: Removing folders without having to format
date: 2009-09-21T01:42:50-07:00
author: joshg253
layout: post
guid: https://gundersons.us/josh/?p=694
permalink: /2009/09/21/removing-folders-without-having-to-format/
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";b:0;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - Uncategorized
---
Win7 on a new drive

want to delete everything but a few folders on the old drive that was used for Vista

In each folder (Program Files, Program Files (x86), Windows, etc.):

takeown /f "Folder Name" /r

cacls * /t /g USERNAME:F