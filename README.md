# My garden

## Mac
* [Clipboard tool](https://github.com/p0deje/Maccy)

## MP3
* Download mp3 `yt-dlp -x --audio-format mp3 https://www.youtube.com/playlist\?list\=PLy5PztYh7B5wOTYl1rH1NzA9zSn2kjXP8`
* Prepare list `ls *.mp3 | sed -e "s/\(.*\)/file '\1'/" | sort > all.txt`
* Merge files `ffmpeg -safe 0 -f concat -i all.txt -c copy all.mp3`

