user-wide fontconfig
===

just put them into your ```$XDG_CONFIG_HOME/fontconfig``` or ```$HOME/.config/fontconfig```

## About $XDG_CONFIG_HOME

And some other "XDG" related environment variables.

now Archlinux will not set them anymore, but we do not need to do anything if we just want to keep them default.

According to [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html#variables "freedesktop.org"):

> If $XDG_CONFIG_HOME is either not set or empty, a default equal to ```$HOME/.config``` should be used.

So that's okay.

## Files in conf.d

from [fontconfig document](https://www.freedesktop.org/software/fontconfig/fontconfig-user.html#AEN79 "freedesktop.org"):

> If a directory, every file within that directory starting with an ASCII digit (U+0030 - U+0039) and ending with the string ``.conf'' will be processed in sorted order.

And if not starting with a digit, e.g. ```family.conf```, will be ignored.