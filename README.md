# bash-task-automation
Scripts I wrote to automate certain tasks on a UNIX system. The files/usage are:

* `record_iOS_simulator [extension]` records an existing iOS Simulator instance with the provided extension (defaults to .mp4) and makes a GIF out of it. Requires Xcode, `ffmpeg`(`brew install ffmpeg`), `gifsicle` (`brew install gifsicle`) and  and a running Simulator.
* `record_iOS_simulatorNO-GIF [extension]` does the same without a GIF.
* `make_GIF filename` takes a file and makes a GIF out of it, assuming it is possible.

Also used [this website](https://iridakos.com/programming/2018/03/01/bash-programmable-completion-tutorial) to add `make_GIF` as a command available wherever and to add autocompletion, and I suggest you do the same ;)
