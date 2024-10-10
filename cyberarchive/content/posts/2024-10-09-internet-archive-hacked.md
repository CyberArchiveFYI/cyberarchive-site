---
title: Internet Archive Hacked, data breach impacts 31 million users
author: Lawrence Abrams
date: 2024-10-09T06:22:00+00:00
draft: false
categories:
  - data-breach
tags:
  - industry_library
---

[Original Article Link](https://www.bleepingcomputer.com/news/security/internet-archive-hacked-data-breach-impacts-31-million-users/)

[Internet Archive Link]()

## Article Paste

Updates added at end of the article.

Internet Archive's "The Wayback Machine" has suffered a data breach after a threat actor compromised the website and stole a user authentication database containing 31 million unique records.

News of the breach began circulating Wednesday afternoon after visitors to archive.org began seeing a JavaScript alert created by the hacker, stating that the Internet Archive was breached.

"Have you ever felt like the Internet Archive runs on sticks and is constantly on the verge of suffering a catastrophic security breach? It just happened. See 31 million of you on HIBP!," reads a JavaScript alert shown on the compromised archive.org site.
JavaScript alert shown on Archive.org
JavaScript alert shown on Archive.org
Source: BleepingComputer

The text "HIBP" refers to is the Have I Been Pwned data breach notification service created by Troy Hunt, with whom threat actors commonly share stolen data to be added to the service.

Hunt told BleepingComputer that the threat actor shared the Internet Archive's authentication database nine days ago and it is a 6.4GB SQL file named "ia_users.sql." The database contains authentication information for registered members, including their email addresses, screen names, password change timestamps, Bcrypt-hashed passwords, and other internal data.

The most recent timestamp on the stolen records is September 28th, 2024, likely when the database was stolen.

Hunt says there are 31 million unique email addresses in the database, with many subscribed to the HIBP data breach notification service. The data will soon be added to HIBP, allowing users to enter their email and confirm if their data was exposed in this breach.

The data was confirmed to be real after Hunt contacted users listed in the databases, including cybersecurity researcher Scott Helme, who permitted BleepingComputer to share his exposed record.

`9887370, internetarchive@scotthelme.co.uk,$2a$10$Bho2e2ptPnFRJyJKIn5BiehIDiEwhjfMZFVRM9fRCarKXkemA3PxuScottHelme,2020-06-25,2020-06-25,internetarchive@scotthelme.co.uk,2020-06-25 13:22:52.7608520,\N0\N\N@scotthelme\N\N\N`

Helme confirmed that the bcrypt-hashed password in the data record matched the brcrypt-hashed password stored in his password manager. He also confirmed that the timestamp in the database record matched the date when he last changed the password in his password manager.
​​​​​​​Password manager entry for archive.org
Password manager entry for archive.org
Source: Scott Helme

Hunt says he contacted the Internet Archive three days ago and began a disclosure process, stating that the data would be loaded into the service in 72 hours, but he has not heard back since.

It is not known how the threat actors breached the Internet Archive and if any other data was stolen.

Earlier today, the Internet Archive suffered a DDoS attack, which has now been claimed by the BlackMeta hacktivist group, who says they will be conducting additional attacks.

SN_BlackMeta tweet

BleepingComputer contacted the Internet Archive with questions about the attack, but no response was immediately available.

Update 10/10/24: Internet Archive founder Brewster Kahle shared an update on X last night, confirming the data breach and stating that the threat actor used a JavaScript library to show the alerts to visitors.

"What we know: DDOS attacked-fended off for now; defacement of our website via JS library; breach of usernames/email/salted-encrypted passwords," reads a first status update tweeted last night.

"What we've done: Disabled the JS library, scrubbing systems, upgrading security."

A second update shared this morning states that DDoS attacks have resumed, taking archive.org and openlibrary.org offline again.

While the Internet Archive is facing both a data breach and DDoS attacks at the same, it is not believed that the two attacks are connected.