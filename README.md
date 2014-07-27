# Source:

<a href="http://www.ibiblio.org/pub/Linux/utils/file/symlinks-1.4.tar.gz">http://www.ibiblio.org/pub/Linux/utils/file/symlinks-1.4.tar.gz</a>

# Description

symlinks: scan/change symbolic links - v1.4 - by Mark Lord

# Usage:

symlinks [-cdorstv] dirlist

# Flags:

* -c == change absolute/messy links to relative
* -d == delete dangling links
* -o == warn about links across file systems
* -r == recurse into subdirs
* -s == shorten lengthy links (displayed in output only when -c not specified)
* -t == show what would be done by -c
* -v == verbose (show all symlinks)

# Change(s)

I just made one change to the original source, so that it can compile on my MacBook Pro:

* In symlinks.c, `#include <malloc.h>` is changed into `#include <malloc.h>`
