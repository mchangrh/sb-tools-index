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
[Invite To Discord](https://sb-slash.mchang.workers.dev/invite)

# client
## sb.js - SB userscript/ bookmarklet
[GitHub](https://github.com/mchangrh/sb.js)  
[GitHub Pages](https://mchangrh.github.io/sb.js/)  

# [Userscripts](https://github.com/mchangrh/uscripts/tree/main/sbltnfi#readme)

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

# static web resources

## sb port matrix
### ports/libraries for sponsorblock and supported categories
URL: [sb.mchang.xyz/ports](https://sb.mchang.xyz/ports)

## sb-openapi
### openAPI documentation for SB API
URL: [openapi.sb.blabdu.de](https://openapi.sb.blabdu.de)  
GitHub: [mchangrh/sb-openapi](https://github.com/mchangrh/sb-openapi)  

## sb-status-chart
### chart for monitoring sb-status-server
URL: [graph.sb.blabdu.de](https://graph.sb.blabdu.de)  
GitHub: [mchangrh/sb-status-chart](https://github.com/mchangrh/sb-status-chart)  

## sb-mirror
### 5 minute mirror of SB database
HTTPS: [mirror.sb.blabdu.de](https://mirror.sb.blabdu.de)  
RSync: `rsync://mirror.sb.blabdu.de/sponsorblock`

## sb gen ID
### generate a random privateID & backup package
GH Pages: [mchangrh/sb-idgen](https://mchangrh.github.io/sb-idgen/)  
GitHub: [mchangrh/sb-idgen](https://github.com/mchangrh/sb-idgen)  

# http servers

## sb-status-server
### nodejs server for monitoring ping of SponsorBlock server
URL: [status.sb.blabdu.de](https://status.sb.blabdu.de)  
GitHub: [mchangrh/sb-status-server](https://github.com/mchangrh/sb-status-server)  
Endpoints:
```
/status - get current response time
/last - get last response time
/all - get last and 5+15 minute averages
```

## sb-userstat-img
### generate userstat images
URL: [img.sb.blabdu.de](https://img.sb.blabdu.de)  
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

## sb-wiki
### docker image and config for SponsorBlock Wiki
GitHub: [mchangrh/sb-wiki](https://github.com/mchangrh/sb-wiki)  
[GHCR](https://github.com/users/mchangrh/packages/container/package/sb-wiki)
`docker pull ghcr.io/mchangrh/sb-wiki:lts`

## sb-wiki-mirror
### docker-compose to mirror the SponsorBlock Wiki
GitHub: [mchangrh/sb-wiki-mirror](https://github.com/mchangrh/sb-wiki-mirror)  
[GH Pages](https://mchangrh.github.io/sb-wiki-mirror/)

![SponsorBlock](./sponsorblock.png)
