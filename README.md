# loop
cause sometimes i need to run stuff in loop

## Usage:
```
usage: loop [-l LOOP_LIMITE] [-i LOOP_INTERVAL] [-t LOOP_TIMER] [-f LOOP_FILE] [-d] COMMAND...
```

## Examples

```
# before going to sleep i run this which play an ASMR video on repeat for 2 hours 
# with an interval of 0.1s, than shutdown my laptop
loop -i 0.1 -t 2h mpv --force-window=no --no-video some_asmr_video.mp4; shutdown --poweroff
```

```
# this recorde a stream with youtube-dl with an interval of 3 minutes 
# and well keep going for 4 hours or 20 round, so i don't get my ip blocked
loop -i 3m -l 20 -t 4h youtube-dl https://stream.url/m.m3u8
```
```
# i run this so i can moniter a log file (interval of 0.2s)
loop -i 0.2 tail /dir/log
# i used this yesterday , when i was trying to connect a device to my laptop
loop -i 0.1 lsusb

```
