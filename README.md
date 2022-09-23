---
title: mchangrh's SB tools index
---

# Index
[discord](#discord)  
[client](#client)  
[userscripts](#userscripts)  
[serverless functions](#serverless-functions)  
[static web resources](#static-web-resources)  
[http servers](#http-servers)  
[misc](#misc)

# discord
## sb-slash
### Discord bot for interacting with SB API

URL: [sb-slash.mchang.workers.dev](https://sb-slash.mchang.workers.dev)  
GitHub: [mchangrh/sb-slash](https://github.com/mchangrh/sb-slash)  
[Invite To Discord](https://sb.mchang.xyz/invite)

# client
## sb.js - SB userscript/ bookmarklet
[GitHub](https://github.com/mchangrh/sb.js)  
[GitHub Pages](https://mchangrh.github.io/sb.js/)  

# userscripts
[Gist](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338)

## sbltnfi
Force refresh a single segment
[Install](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338/raw/sbltnfi-refresh.user.js)

Add sb.mchang.xyz link to entries
[Install](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338/raw/sbltnfi-requiredSegments.user.js)

Remove trailing zeroes from start, end and length times
[Install](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338/raw/sbltnfi-imprecise-times.user.js)

Fork of NanoByte's clickable starttime Script with more aggressive videoID searching
[Install](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338/raw/sbltnfi-clickable-starttime-fork.user.js)

Fork of Deedit's sb.ltn.fi/video/-Opener with preset filters
[Install](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338/raw/sbltnfi-preset-video-link.user.js)

Replaces or redirct all sb.ltn.fi links to be pre-loaded with filters
[Install](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338/raw/sbltnfi-preset-replace.user.js)

Add Discord badge to any users that are registered with sb-slash
[Install](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338/raw/sbltnfi-discord-badge.user.js)

Fork of TheJzoli's videotitles with searching done through innertube
[Install](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338/raw/sbltnfi-it-videotitle.user.js)

## youtube
Adds a big red warning to the top of the screen when requiredSegment(s) are present
[Install](https://gist.github.com/mchangrh/9507604353e37b6abc2f7f6b3c6e1338/raw/yt-warn-reqseg.user.js)

# serverless functions
## sb-lookup
### SponsorBlock UUID to YouTube link
URL: [sb.mchang.xyz/](https://sb.mchang.xyz)  
GitHub: [mchangrh/sb-lookup](https://github.com/mchangrh/sb-lookup)  
Endpoints:
```
/<uuid> - redirect to YouTube link
/<uuid>/<option> - option can be - db | info | video 
?api=false - if truthy, return JSON instead of redirect 
```

## webcrypto-hash
### derive publicID from privateID
URL: [hash.mchang.workers.dev](https://hash.mchang.workers.dev)  
GitHub: [mchangrh/webcrypto-hash](https://github.com/mchangrh/webcrypto-hash)  
Query Parameters
```
input=<privateID>
times=<number of times to hash> (default 5000)
algo=<algorithm to use> (default SHA-256)
```

## sb-logos
### derivative SponsorBlock logos
URL: [sb-logo.mchang.workers.dev](https://sb-logo.mchang.workers.dev)  
GitHub: [mchangrh/sb-logos](https://github.com/mchangrh/sb-logos)

# static web resources

## sb port matrix
### ports/libraries for sponsorblock and supported categories
URL: [mchang.icu/sb-matrix](https://mchang.icu/sb-matrix)

## sb-openapi
### openAPI documentation for SB API
URL: [sb-openapi.mchang.icu](https://sb-openapi.mchang.icu)  
GitHub: [mchangrh/sb-openapi](https://github.com/mchangrh/sb-openapi)  

## sb-status-chart
### chart for monitoring sb-status-server
URL: [mchangrh.github.io/sb-status-chart](https://mchangrh.github.io/sb-status-chart)   
GitHub: [mchangrh/sb-status-chart](https://github.com/mchangrh/sb-status-chart)  

## sb-mirror
### 5 minute mirror of SB database
HTTPS: [mirror.sb.mchang.xyz](https://mirror.sb.mchang.xyz)  
RSync: `rsync://mirror.sb.mchang.xyz/sponsorblock`

## sb-archive
### historical archive of SB Database
HTTPS (CloudFlare): [https://archive.sb.mchang.xyz](https://sb-archive.mchang.xyz)  
HTTP (Direct): [http://qc.mchang.xyz](http://qc.mchang.xyz)  
RSync: `rsync://qc.mchang.icu/sponsorblock`  
GitHub: [mchangrh/sb-archive](https://github.com/mchangrh/sb-archive)

## sb gen ID
### generate a random privateID & backup package
URL: [id.sb.mchang.xyz](https://id.sb.mchang.xyz)
GH Pages: [mchangrh/sb-idgen](https://mchangrh.github.io/sb-idgen/)
GitHub: [mchangrh/sb-idgen](https://github.com/mchangrh/sb-idgen)

# http servers

## sb-status-server
### nodejs server for monitoring ping of SponsorBlock server
URL: [status.sb.mchang.xyz](https://status.sb.mchang.xyz)  
GitHub: [mchangrh/sb-status-server](https://github.com/mchangrh/sb-status-server)  
Endpoints:
```
/status - get current response time
/last - get last response time
/all - get last and 5+15 minute averages
```

## sb-userstat-img
### generate userstat images
URL: [img.sb.mchang.xyz](https://img.sb.mchang.xyz)  
GitHub: [mchangrh/sb-userstat-img](https://github.com/mchangrh/sb-userstat-img)  
Endpoints: 
```
/pie?userID=<publicUserID>
generate pie chart of submission categories

/stats?userID=<publicUserID>
generate stats image
```

## sb-ml-api
### API for segment suggestions from [xenova/sponsorblock-ml](https://github.com/xenova/sponsorblock-ml)
URL: `Not for public use`
GitHub: [mchangrh/sb-ml-api](https://github.com/mchangrh/sb-ml-api)
Endpoints:
```
/get
/done
/reject
/load
```

# Misc

## sb-category-type
### nodejs constants for category types
GitHub: [mchangrh/sb-category-type](https://github.com/mchangrh/sb-category-type)  
NPM: https://www.npmjs.com/package/sb-category-type

## sb-mirror
### docker images to mirror SB database
GitHub: [mchangrh/sb-mirror](https://github.com/mchangrh/sb-mirror)  
[DockerHub](https://hub.docker.com/r/mchangrh/sb-mirror):
`docker pull mchangrh/sb-mirror`  
[GHCR](https://github.com/mchangrh/sb-mirror/pkgs/container/sb-mirror):
`docker pull ghcr.io/mchangrh/sb-mirror`


![SponsorBlock](./sponsorblock.png)
