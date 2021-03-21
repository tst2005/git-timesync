# git-timesync

When you `git clone` a repository, the lastmod timestamps of the created files are set to the current date and time. This script allows you to synchronize the **lastmod timestamps** of the files in the **working tree** from the **commit** times of the Git repository.

## Installation

The easiest way to install (or update) this script on your computer is to download and place it in a directory in your `$PATH` and `chmod +x` it.

Suppose that we want to place it in the `$HOME/bin` folder; to do so, you can just execute the following Bash commands:

```bash
curl -o "$HOME/bin/git-timesync" https://raw.githubusercontent.com/tst2005/git-timesync/master/git-timesync
chmod +x "$HOME/bin/git-timesync"
```

## Usage

Make a fresh clone of a Git repository of your choice:

```bash
git clone GIT_REPOSITORY_URL
```

See what is needed to sync with:

```bash
git timesync -n
```

If you want to drop everything that is OK and see only what is needed to sync, use:

```bash
git timesync -n -q
```

If you want to apply all the changes, use:

```bash
git timesync
```

If you want apply a change only to one file, use:

```bash
git timesync THE_WANTED_FILE
```

## License

I usually release my code under the *MIT license*, but I will follow the original author's one.
