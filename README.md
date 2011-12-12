# What

skel-complete generates bare-bones bash completion files for a given command, produced by pulling out options from the man page. It's basically a toy, and it relies on one hell of a regular expression.

# Installing

Grab `skel-complete` and place it somewhere in your `PATH`. You'll need Ruby.

# Usage

	$ skel-complete <command> > ~/etc/<command>-completion.bash
	$ . ~/etc/<command>-completion.bash

e.g., if `<command>` is `rsync`:

	$ skel-complete rsync > ~/etc/rsync-completion.bash
	$ . ~/etc/rsync-completion.bash

After that, `rsync --vers<TAB>` will tab complete, as will any other option successfully retrieved from the man page of `<command>`.

# License

Copyright (c) 2011 Adam Prescott. Released under the MIT license. See the license file.

# TODO

Drop the Ruby dependency.
