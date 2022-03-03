# Index
[discord](#discord)  
[static web resources](#static-web-resources)  
[serverless functions](#serverless-functions)  
[http servers](#http-servers)  
[misc](#misc)

# discord
## sb-slash
### Discord bot for interacting with SB API

URL: [sb-slash.mchang.workers.dev](https://sb-slash.mchang.workers.dev)  
GitHub: [mchangrh/sb-slash](https://github.com/mchangrh/sb-slash)  
[Invite To Discord](https://sb.mchang.xyz/invite)

# serverless functions
## sb-lookup
## SponsorBlock UUID to YouTube link
URL: [sb.mchang.xyz/](https://sb.mchang.xyz)  
GitHub: [mchangrh/sb-lookup](https://github.com/mchangrh/sb-lookup)  
Endpoints:
```
/<uuid> - redirect to YouTube link
/<videoid>/<partialuuid> - partial uuid lookup
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
HTTPS: [sb-mirror.mchang.xyz](https://sb-mirror.mchang.xyz)  
RSync: `rsync://sb-mirror.mchang.xyz/sponsorblock`

## sb-archive
### historical archive of SB Database
HTTPS (CloudFlare): [https://sb-archive.mchang.xyz](https://sb-archive.mchang.xyz)  
HTTP (Direct): [http://qc.mchang.xyz](http://qc.mchang.xyz)  
RSync: `rsync://qc.mchang.icu/sponsorblock`  
GitHub: [mchangrh/sb-archive](https://github.com/mchangrh/sb-archive)

# http servers

## sb-status-server
### nodejs server for monitoring ping of SponsorBlock server
URL: [sb-status.mchang.xyz](https://sb-status.mchang.xyz)  
GitHub: [mchangrh/sb-status-server](https://github.com/mchangrh/sb-status-server)  
Endpoints:
```
/status - get current response time
/last - get last response time
/all - get last and 5+15 minute averages
```

## sb-userstat-img
### generate userstat images
URL: [sb-img.mchang.xyz](https://sb-img.mchang.xyz)  
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

## sbb-requiredSegments
### required segment userscript for sb.ltn.fi
[URL](https://gist.github.com/mchangrh/603db65fd7dfc177a0eb21cef4ca8270/raw/sbltnfi-requiredSegments.user.js) | 
[Gist](https://gist.github.com/mchangrh/603db65fd7dfc177a0eb21cef4ca8270)  

## sbb-refresh
### refresh segment userscript for sb.ltn.fi
[URL](https://gist.github.com/mchangrh/c693f8e1de2b6a5067ae9d5e994f6758/raw/sbltnfi-refresh.user.js) |
[Gist](https://gist.github.com/mchangrh/c693f8e1de2b6a5067ae9d5e994f6758)

## sb-mirror
### docker images to mirror SB database
GitHub: [mchangrh/sb-mirror](https://github.com/mchangrh/sb-mirror)  
[DockerHub](https://hub.docker.com/r/mchangrh/sb-mirror):
`docker pull mchangrh/sb-mirror`  
[GHCR](https://github.com/mchangrh/sb-mirror/pkgs/container/sb-mirror):
`docker pull ghcr.io/mchangrh/sb-mirror`
