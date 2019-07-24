# downloadYoutube, youtube-dl for humans ;)
This Script is intended to be a friendly "frontend" for youtube-dl which automatically download the higher definition available

**youtube-dl** project
https://rg3.github.io/youtube-dl/

## 1. Install
### (ffmpeg) it is mandatory to join video and audio in one file

*(debian / ubuntu)* `sudo apt install ffmpeg`

*(centos / redhat)* `sudo yum install ffmpeg`

*(archlinux (mainstream))* `sudo pacman -S ffmpeg`

*(manual install)* `https://pkgs.org/download/ffmpeg`

### (youtube-dl)

*(debian / ubuntu)* `sudo apt install youtube-dl`

*(centos / redhat)* `sudo yum install youtube-dl`

*(archlinux (mainstream))* `sudo pacman -S youtube-dl`

*(manual install)* `sudo wget https://yt-dl.org/downloads/latest/youtube-dl -O /usr/local/bin/youtube-dl`

### (downloadYoutube)
`sudo wget https://raw.githubusercontent.com/G3NSVRV/downloadYoutube/master/downloadYoutube -O /usr/local/bin/downloadYoutube`

### (add executable properties)
`sudo chmod a+rx /usr/local/bin/youtube-dl /usr/local/bin/downloadYoutube`

## 2. Usage
`$: downloadYoutube $video_url`

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
