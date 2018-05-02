# gifvid
Converts a GIF to an MP4 using ffmpeg.

Based on the blog [Replace Animated GIFs with Video](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/replace-animated-gifs-with-video/) by Jeremy Wagner.

### Why?

Because the command given in the blog produces a video that is not supported by Safari and Firefox. The right command is long and needs an alias to be set up unless you have genius level memory.

### Installation

* Install ffmpeg(`brew install ffmpeg` on macOS).
* Clone the repo.
* Run `chmod +x gifvid`.
* Copy this to the bin path by running `cp gifvid /usr/bin`. Use `sudo` if needed.

### Usage

`gifvid source`

`source` is mandatory. The converted video will be written to `source.mp4`.

### CLI Flags

`-s`
`--src` - Specify the source.

`-d`
`--dest` - Specify the destination. Will be `source.mp4` if not given.

`-c`
`--crf` - Constant Rate Factor. Defaults to `25`. Lower the number, higher the quality and file size.
