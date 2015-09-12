git timesync
============

When you make a git clone the created file are the current date.
This script allow you to change the file timestamp to the same than the repository one.

How to install it
=================

Clone this repository
```
git clone https://github.com/tst2005/git-timesync
```
or download the git-timesync file
```
wget https://github.com/tst2005/git-timefix/blob/master/bin/git-timesync
```

Add it in the git path :

```
FIXME how to do what ?
```

Or use the `./git-timesync` instead of `git timesync`


How to use it
=============

Make a fresh clone of any git repository with `git clone SOME_GIT_REPOSITORY_URL`

See what is needed to sync with `git timesync -n`

If you want drop everything that is ok and see only what is needed to sync, use `git timesync -n -q`

If you want apply all change, use `git timesync`

If you want apply change only in one file, use `git timesync THE_WANTED_FILE`

License
=======

I usualy release my code under MIT license, but I will follow the original author's one.
