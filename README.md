# bash-task-automation
Scripts I wrote to automate certain tasks on a UNIX system. The files/usage are:

* `film_simulator [extension]` records an existing iOS Simulator instance with the provided extension (defaults to .mp4) and makes a GIF out of it. Requires Xcode, `ffmpeg`(`brew install ffmpeg`), `gifsicle` (`brew install gifsicle`) and  and a running Simulator.
* `film_simulatorNo_GIF [extension]` does the same without a GIF.
* `make_GIF filename` takes a file and makes a GIF out of it, assuming it is possible.
