# gifvid
Converts a GIF to an MP4 using ffmpeg.

Based on the blog [Replace Animated GIFs](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/replace-animated-gifs-with-video/) with Video by Jeremy Wagner.

### Why?

Because the command given in the blog produces a video that is not supported by Safari and Firefox. The right command is long and needs an alias to be set up unless you have genius level memory.

### Installation

* Install ffmpeg(`brew install ffmpeg` on macOS).
* Clone the repo.
* Run `chmod +x gifvid`.
* Copy this to the bin path by running `cp gifvid /usr/bin`. Use `sudo` if needed.

### Usage

`gifvid source destination`

`source` is mandatory. If `destination` is not given, the converted video will be written to `source.mp4`.
