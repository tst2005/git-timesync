# git-timesync

When you `git clone` a repository, the last modification timestamps of the created files are set to the current date and time. This script allows you to synchronize the **last modification timestamps** of the files in the **working tree** from the **commit** times of the Git repository.


## Installation

Clone this repository
```
git clone https://github.com/tst2005/git-timesync
```
or download the git-timesync file
```
wget https://github.com/tst2005/git-timesync/raw/master/bin/git-timesync
```

For it to be found by git, you need to install it in a directory in your `$PATH`.
For user installation (no root needed, will only work for current user) we recommend `~/.local/bin`. You can add the following to your `.bashrc` or `.zshrc` if you don't already have it configured.

```sh
export PATH=~/.local/bin:$PATH
```
Then just move `git-timesync` to `~/.local/bin/`.

For system-wide installation, move it to something that's in the path of all users. We recommend `/usr/local/bin/`.


## Usage

Make a fresh clone of a Git repository of your choice:

```sh
git clone GIT_REPOSITORY_URL
```

See which files are OK and which ones need to be synchronized (**dry-run**) with:

```sh
git timesync --dry-run
```

If you want to drop everything that is OK and show **only** the files which timestamp **needs to be synchronized**:

```sh
git timesync --dry-run --quiet
```

If you want to **apply all the changes**, use:

```sh
git timesync
```

If you want **apply a change only to one file**, use:

```sh
git timesync THE_WANTED_FILE
```

If you want to view the **help message**:

```sh
git timesync --help
```

License
=======

The original author's did not answer after 6 years about the license of his code.
Years after years, I almost rewrote the whole script and implement new feature and large improvement, then I decided of the license.

This projet is release under the *MIT license*.
