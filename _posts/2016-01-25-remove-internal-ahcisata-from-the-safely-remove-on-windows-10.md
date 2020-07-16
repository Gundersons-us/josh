---
id: 1467
title: Remove internal AHCI/SATA from the Safely Remove on Windows 10
date: 2016-01-25T16:43:43-08:00
author: joshg253
layout: post
guid: http://gundersons.us/josh/?p=1467
permalink: /2016/01/25/remove-internal-ahcisata-from-the-safely-remove-on-windows-10/
slide_template:
  - default
fw_options:
  - 'a:2:{s:22:"seo-titles-metas-title";s:0:"";s:28:"seo-titles-metas-description";s:0:"";}'
categories:
  - Uncategorized
---
I have my motherboard set to use devices as AHCI, and all my SATA drives show up under the Safely Remove icon in Windows 10. Since I rarely need to remove the boot SSD while I'm actively using the computer, I don't want to see it or any of the other internal drives in that menu.

Run RegEdit and navigate to:
<p style="padding-left: 30px;">HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\storahci\Parameters\Device</p>
Add a new Multi String Value called TreatAsInternalPort set the value like so (I have 8 internal drives I want to hide, so 0-7):
<pre>0
1
2
4
5
6
7

</pre>
(note the newlines after each number, including the last one)

Found here: http://superuser.com/questions/12955/how-can-i-remove-the-option-to-eject-sata-drives-from-the-windows-7-tray-icon/961242#961242