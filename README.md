# stream-rip-restart

## Bash script for `streamripper` - Restarts `streamripper` for the left recording time if it quits too early

If `streamripper` exits too early, before the specified recording time (streamripper option `-l`) is over (maybe because of an interrupted internet connection or other problems), not everything what you wanted to record is ripped. You will stay there with only a part of the radio program you were interested in :-(

To avoid that you can use this little Bash script. It restarts `streamripper` automatically so often if the specified recording length is reached.

## Usage
```
$ streamrip.sh URL DIRECTORY FILENAME MINUTES
```
`streamrip.sh` will create specified DIRECTORY and inside it there will be the ripped file with name FILENAME. Current date and time will be appended to FILENAME automatically.

MINUTES is the recording length in minutes.

URL is the link to the stream address.
