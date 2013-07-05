## Dropbox Sync Toggle

### About
An [Alfred][http://www.alfredapp.com/] workflow for quickly disabling Dropbox syncing.  Some use cases:

- You are running on battery and don't want Dropbox draining your charge
- You are editing large files and don't want them sync'd until you are finished
- You are moving many files into Dropbox and don't want them sync'd immediately

### Install
After downloading the workflow file named *dropbox-sync-toggle.alfredworkflow*, you can either double click the file to install or drag-n-drop into the Alfred workflow list in preferences.

[\[Download link\]][0]

### Usage
The default hotkey is `db`.  Hit return and a message will appear via Growl/Notifications with the action taken.

### Behind the Curtain
This workflow leverages the SIGSTOP and SIGCONT [Unix process signals][1].  SIGSTOP is equivalent to hitting C-z while running a script in the terminal, and SIGCONT is equivalent to typing `fg` to resume.

### TODO
- Add `db status` to show the current state

### Annoyances
- The Dropbox icon doesn't show the current state.

### License
Copyright (C) 2013 Kevin McFadden

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[0]: https://github.com/n3bulous/dropbox-sync-toggle/raw/master/Downloads/dropbox-sync-toggle.alfredworkflow
[1]: https://en.wikipedia.org/wiki/Unix_signal
