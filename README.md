# FFmpeg usefull commands:
<br>
1) Convert mkv and add subtitle to a mp4 video
<br>
ffmpeg -i video.mkv -vf subtitles=subtitle.srt -c:v libx264 -c:a aac -strict -2 videowithembedsubtitle.mp4
<br><br>
2) Embed subtitle into mkv<br>
ffmpeg -i video.mkv -vf subtitles=subtitle.srt embed.mkv
<br><br>
3)convert mkv into mp4 with ffpmeg
ffmpeg -i video.mkv -c:v libx264 -c:a aac -strict -2 output_video.mp4
