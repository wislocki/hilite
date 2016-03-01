# hilite

`hilite` is a simple Ruby highlighting (colorizing) script to pipe
things through. 

I've included a couple sample settings files, `hilite-mvn` and `hilite-logs`, along with scripts that I use to pipe output from [Maven](https://maven.apache.org/) or log files through `hilite`.

A settings file is nothing more than a big ruby array of regex-color
pairs (or regex-color-effect triplets) that the `hilite` loads
and uses to mark the matching piped-in text with the appropriate ASCII
color escape code.

My Ruby is pretty rusty, and I'm sure there are tons of better ways to
do this, but it works for me.

Daniel

P.S. The settings files that I've included are set to match the following output format from [log4j 1.2](https://logging.apache.org/log4j/1.2/):

```properties
log4j.appender.R.layout=org.apache.log4j.PatternLayout
log4j.appender.R.layout.ConversionPattern=%d{EEE MMM dd HH:mm:ss.SSS zzz yyyy} - %C.%M() - %t%n%p: %m%n
```
