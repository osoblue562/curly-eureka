  "BLACK_AND_GOLD_FULL.mp4"
ffmpeg -stream_loop -1 -i "pittsburgh_fan_visual.mp4" \
  -i "DBMG PRESENTS...BLACK & GOLD MODE.mp3" \
  -map 0:v:0 -map 1:a:0 \
  -c:v libx264 -c:a aac -b:a 192k \
  -pix_fmt yuv420p \
  "BLACK_AND_GOLD_FULL.mp4"
  
  
