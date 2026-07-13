---
title: "Containers: pitfalls of incomplete tar archives"
url: "https://bootc.dev/blog/2025-dec-15-blog-containers-pitfalls-of-incomplete-tar-archives/"
date: "2025-12-15"
author: ""
feed_url: "https://bootc.dev/rss.xml"
---
Containers: pitfalls of incomplete tar archives As Colin Walters likes to say, containers are just tarballs wrapped in JSON. We'll mostly ignore the JSON part here, but there's a lot to unpack (pun and foreshadowing intended) with regards to tar and how it interacts with the various pieces that work in conjunction to make containers a reality. A refresher on tar Let's explore a key quirk of tar from which everything else we'll discuss follows.
