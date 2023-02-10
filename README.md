# FFmpeg usefull commands:

1) Convert mkv and add subtitle to a mp4 video
ffmpeg -i video.mkv -vf subtitles=subtitle.srt -c:v libx264 -c:a aac -strict -2 videowithembedsubtitle.mp4

2) Embed subtitle into mkv
ffmpeg -i video.mkv -vf subtitles=subtitle.srt embed.mkv

3)convert mkv into mp4 with ffpmeg
ffmpeg -i video.mkv -c:v libx264 -c:a aac -strict -2 output_video.mp4
