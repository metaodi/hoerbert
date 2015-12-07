#!/bin/bash

cdparanoia -B

INDEX=0
for TRACK in *.wav; do
  sox --buffer 131072 --multi-threaded --no-glob $TRACK --clobber -r 32000 -b 16 -e signed-integer --no-glob ${INDEX}.WAV remix - gain -n -1.5 bass +1 loudness -1 pad 0 0 dither
  INDEX=$((${INDEX}+1))
  rm $TRACK
done
