# bash-task-automation

Scripts I wrote to automate certain tasks on a *NIX system. The files/usage are:

## Recording

Require ffmpeg(`brew install ffmpeg`) and gifsicle (`brew install gifsicle`).

* `make_GIF filename` takes a file and makes a GIF out of it, assuming it is possible.
* `record_iOS_simulator [extension]` records an existing iOS Simulator instance with the provided extension (defaults to .mp4) and makes a GIF out of it. Requires Xcode and a running simulator.
* `record_iOS_simulatorNO-GIF [extension]` does the same as above but without a GIF.

Also used [this website](https://iridakos.com/programming/2018/03/01/bash-programmable-completion-tutorial) to add `make_GIF` as a command available wherever and to add autocompletion, and I suggest you do the same:

1. `sudo install ./make_GIF /usr/local/bin/make_GIF` (make sure `usr/local/bin` is added to the PATH)

2. `nano make_GIF-completion.bash`

3. ```
    #/usr/bin/env bash
    complete -A directory make_GIF
    ```
