---
id: 1470
title: Pidgin + Google Apps for Your Domain with 2-factor Authentication
date: 2016-01-25T22:08:47-08:00
author: joshg253
layout: post
guid: https://gundersons.us/josh/?p=1470
permalink: /2016/01/25/pidgin-google-apps-for-your-domain-with-2-factor-authentication/
slide_template:
  - default
fw_options:
  - 'a:2:{s:22:"seo-titles-metas-title";s:0:"";s:28:"seo-titles-metas-description";s:0:"";}'
categories:
  - Uncategorized
---
<ol>
 	<li>Create an app-specific password for Pidgin: <a href="https://security.google.com/settings/security/apppasswords">https://security.google.com/settings/security/apppasswords</a></li>
 	<li>Add a new account in Pidgin:
<ul>
 	<li>Basic tab:
<ul>
 	<li>Protocol: Google Talk or XMPP</li>
 	<li>Username: {yourusername}</li>
 	<li>Domain: {yourdomain.tld}</li>
 	<li>Resource: {left blank}</li>
 	<li>Password: {app-specific password}</li>
 	<li>Remember password: Checked</li>
</ul>
</li>
 	<li>Advanced tab:
<ul>
 	<li>Connection security: Use Old-style SSL</li>
 	<li>Connect port: 443</li>
 	<li>Connect server: talk.google.com</li>
 	<li>File transfer proxies: proxy.eu.jabber.org (the default)</li>
</ul>
</li>
</ul>
</li>
</ol>
Hat-tip: <a href="https://superuser.com/a/894407">https://superuser.com/a/894407</a>