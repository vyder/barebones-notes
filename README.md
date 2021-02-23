# Notes. And nothing else.


I've been wanting a notes app I can use in the terminal on my Ubuntu server for
a while. Every few months I forget how to do mundane things like find reverse dependencies
for a package, or uninstall something including rc files, and the classic what are
certbot's arguments again??, etc.

I embarked on making [this ncurses terminal app](https://github.com/vyder/terminal-notes) for that purpose,
but it got too complicated to start using immediately.

This is my solution, and my notes.


## Installation

1. Fork this repo, and clear out the _notes.txt, or keep it if you want my notes 🤷🏽‍♂️
2. Run `./install` - which will symlink `~/_notes.txt` and `~/bin/notes`

## Usage

My main use cases are:

1. Browse the notes:
   ```
   ❯ notes
   ```
   This opens the notes in `less`


2. Add a new note:
   ```
   ❯ notes
   # Hit `v` to open your default editor
   # Hit `q` twice to exit
   # (Once for my editor `nano`, once to exit `less`)
   ```   

3. Search for a keyword:
   ```
   ❯ notes purge
   # To search for 'purge'
   # Use `n` and `N` to go forward/backward through results
   ```

You can read more about how to use `less` and other tips/tricks in [this great article](https://www.howtogeek.com/444233/how-to-use-the-less-command-on-linux/).


