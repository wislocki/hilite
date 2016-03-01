# hilite

Hilite is a simple Ruby highlighting (colorizing) script to pipe
things through. 

I've included a sample settings file, hilite-mvn, along with a script
that I use to pipe output from Maven through hilite.

The settings file is nothing more than a big ruby array of regex-color
pairs (or regex-color-effect triplets) that the hilite script loads
and uses to mark the matching piped-in text with the appropriate ASCII
color escape code.

My ruby is pretty rusty, and I'm sure there are tons of better ways to
do this, but it works for me.

Daniel
