# Setup

The LFTP community has ported LFTP to a variety of operating systems through a collection of automated packages. If you have used `apt-get` or `yum` before, you will be familiar with this process. If not, you may want to practice installing software via command line package managers.

## Compile from source code

LFTP is free and open source, hosted at http://lftp.yar.ru/. If you want to manually compile and install LFTP from raw source code, you are free to do so under the GNU Public License.

## Package Managers

### Mac OS X

Mac users can install LFTP with the [Homebrew](http://brew.sh/) package manager. If you have not installed Homebrew yet, you will want to follow the instructions at http://brew.sh/#install before continuing.

After Homebrew is installed, enter `brew install lftp` to install LFTP.

### Windows

Windows users can install LFTP with the [Chocolatey](https://chocolatey.org/) package manager. If you have not installed Chocolatey yet, you will want to follow the instructions at https://chocolatey.org/ before continuing.

After Chocolatey is installed, enter `chocolatey install lftp` to install LFTP.

### Debian, Ubuntu, Raspbian, etc.

Debian-based Linux distributions can install LFTP with `sudo apt-get install lftp`.

### RedHat, Fedora, CentOS, etc.

RedHat-based distributions can install LFTP with `sudo yum install lftp`.

### Gentoo

Gentoo users can install LFTP with `emerge lftp`.

## Configuration

LFTP provides a reasonable set of defaults out of the box, but eventually, you may want to tweak LFTP to fit your workflow better.

To configure LFTP, edit `$HOME/.lftprc` with a text editor such as `nano` or [Atom](https://atom.io/).

Example `.lftprc`: https://github.com/mcandre/dotfiles/blob/master/.lftprc