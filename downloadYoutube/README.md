# downloadYoutube, yt-dlp for humans ;)
This Script is intended to be a friendly "frontend" for ~youtube-dl~ yt-dlp which automatically download the higher definition available

** update **
I changed the main binary from youtube-dl to yt-dlp because has better download speeds; yt-dlp is a fork of youtube-dl plus extra features that can be used on future releases of this script.

**yt-dlp** project
https://github.com/yt-dlp/yt-dlp

## 1. Dependencies
### (ffmpeg) is mandatory to merge video and audio in one file:

*(debian / ubuntu)* `sudo apt install ffmpeg`

*(centos / redhat)* `sudo yum install ffmpeg`

*(archlinux (mainstream))* `sudo pacman -S ffmpeg`

*(manual install)* `https://pkgs.org/download/ffmpeg`

### (yt-dlp):

https://github.com/yt-dlp/yt-dlp#installation

## 2. Installation

### (downloadYoutube):
`sudo wget https://raw.githubusercontent.com/G3NSVRV/PowerUserScripts/master/downloadYoutube/downloadYoutube -O /usr/local/bin/downloadYoutube`

### (add executable properties):
`sudo chmod a+rx /usr/local/bin/downloadYoutube`

## 3. Usage
```
$: downloadYoutube $videoUrl
```

#### example:
```
$: downloadYoutube https://www.youtube.com/watch?v=XCspzg9-bAg
Descargando en LD
[youtube] XCspzg9-bAg: Downloading webpage
[youtube] XCspzg9-bAg: Downloading video info webpage
[download] Destination: Batroll'd.f133.mp4
[download] 100% of 1.59MiB in 00:00
[download] Destination: Batroll'd.f171.webm
[download] 100% of 619.03KiB in 00:00
[ffmpeg] Merging formats into "Batroll'd.mp4"
Deleting original file Batroll'd.f133.mp4 (pass -k to keep)
Deleting original file Batroll'd.f171.webm (pass -k to keep)
```

## Known Bugs
#### Cannot download Playlists. This should be fixed soon :)
