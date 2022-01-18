## sb-slash
### Discord bot for interacting with SB API

URL: https://sb-slash.mchang.workers.dev  
GH: https://github.com/mchangrh/sb-slash  
Endpoints:
```
/invite - invite the bot
/github - link to the github repo
```

## sb-lookup
## SponsorBlock UUID to YouTube link
URL: https://sb.mchang.xyz  
GH: https://github.com/mchangrh/sb-lookup  
Endpoints:
```
/<uuid> - redirect to YouTube link
/<videoid>/<partialuuid> - partial uuid lookup
?api=false - if truthy, return JSON instead of redirect 
```

## sb port matrix
### ports/libraries for sponsorblock and supported categories
URL: https://mchang.icu/sb-matrix

## sb-openapi
### openAPI documentation for SB API
URL: https://sb-openapi.mchang.icu  
GH: https://github.com/mchangrh/sb-openapi  

## sb-status-server
### nodejs server for monitoring ping of SponsorBlock server
URL: https://sb-status.mchang.xyz  
GH: https://github.com/mchangrh/sb-status-server  
Endpoints:
```
/status - get current response time
/last - get last response time
/all - get last and 5+15 minute averages
```

## sb-status-chart
### chart for monitoring sb-status-server
URL: https://mchangrh.github.io/sb-status-chart   
GH: https://github.com/mchangrh/sb-status-chart  

## sb-userstat-img
### generate userstat images
URL: https://sb-img.mchang.xyz  
GH: https://github.com/mchangrh/sb-userstat-img  
Endpoints: 
```
/pie?userID=<publicUserID>
generate pie chart of submission categories

/stats?userID=<publicUserID>
generate stats image
```

## sbb-requiredSegments
### required segment userscript for sb.ltn.fi
URL: https://gist.github.com/mchangrh/603db65fd7dfc177a0eb21cef4ca8270/raw/sbltnfi-requiredSegments.user.js  
GH: https://gist.github.com/mchangrh/603db65fd7dfc177a0eb21cef4ca8270  

## sb-mirror
### docker images to mirror SB database
GH: https://github.com/mchangrh/sb-mirror

## sb-mirror
### 5 minute mirror of SB database
HTTPS: https://sb-mirror.mchang.xyz  
RSync: `rsync://sb-mirror.mchang.xyz/sponsorblock`

## sb-archive
### historical archive of SB Database
HTTPS (CF): https://sb-archive.mchang.xyz  
HTTP (Direct): http://qc.mchang.xyz  
RSync: `rsync://qc.mchang.icu/sponsorblock`  
GH: https://github.com/mchangrh/sb-archive  

## webcrypto-hash
### derive publicID from privateID
URL: https://hash.mchang.workers.dev  
GH: https://github.com/mchangrh/webcrypto-hash  
Query Parameters
```
input=<privateID>
times=<number of times to hash> (default 5000)
algo=<algorithm to use> (default SHA-256)
```
