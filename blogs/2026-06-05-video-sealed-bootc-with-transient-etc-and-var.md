---
title: "Video: sealed bootc with transient /etc and /var"
url: "https://bootc.dev/blog/2026-jun-05-transient-root-etc-var/"
date: "2026-06-05"
author: ""
feed_url: "https://bootc.dev/rss.xml"
---
Video: sealed bootc with transient /etc and /var I recorded a short demo of the new composefs mount configuration support that landed in bootc#2201 . The PR adds a /usr/lib/bootc/setup-root-conf.toml file that image authors can ship in their container image to control how the composefs-backed root filesystem is mounted at boot: [root] transient = true wraps the composefs lower in a tmpfs overlay, so all writes to / are discarded on reboot. [etc] mount = "transient"|"overlay"|"bind"|"none" controls how /etc is mounted from the deployment state directory.
