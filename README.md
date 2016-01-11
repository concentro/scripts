A place to share scripts.

Mostly created to help fix minor annoyances when using certain websites.

## Structure ##

    .
    ├── bin
    └── local
        └── bin

* bin: scripts intended to run on most Linux distributions
* local/bin: scripts limited by local dependencies

Dependencies could be:

* needs further software not available by default on most Linux distributions. See the script's help (`script.sh -h`)
* uses data at specified paths on the local machine. See the script's help (`script.sh -h`)

## Installation ##

1. Download locally to a directory of your choice, for example your home directory: `~/scripts`
2. Include `bin` directories in your `$PATH`. For example append and save in `~/.bash_aliases`:

    export PATH="$HOME/scripts/bin:$HOME/scripts/local/bin:$PATH"

3. source bash or start a new terminal for the update to be effective:

    $ . ~/.bashrc

4. To run a script named `script.sh`:

    $ script.sh

## Misc ##

Started 2015-12-16
