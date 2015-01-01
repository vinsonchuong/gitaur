# gitaur-pkgbuild(1) -- populates an incomplete PKGBUILD

## SYNOPSIS
`gitaur-pkgbuild` <PKGBUILD><br>
`gitaur-pkgbuild` `-h`|`--help`<br>

## DESCRIPTION
`gitaur-pkgbuild` populates an incomplete `PKGBUILD` with values derived from
the corresponding GitHub repository and AUR deployment.

The default values used are as follows:

* `pkgname` the name of the GitHub repository
* `pkgver` is the most recent tag, assumed to follow the format `vX.Y.Z`
* `pkgrel` is `1` if a new version is being uploaded to the AUR and the
  current AUR release's `pkgrel` incremeted otherwise
* `pkgdesc` is the description of the GitHub repository
* `arch` is `any`
* `url` is the GitHub repository's URL
* `license` is computed by parsing the `LICENSE` file in the root of the
  repository
* `source` is an archived version of the most recent tag as described above
* `md5sums` is computed using `makepkg -g`

A default `build` function is provided that runs `clidoc` on the
contents of the `doc` directory if it exists.

Also, a default `package` function is provided that automatically installs
files that follow the directory structure:

* `bin` containing only executables with no sub-directories
* `help` text generated above by `clidoc`
* `man` containing `*.1` man pages
* `README.md`
* `LICENSE`

## OPTIONS
* -h, --help:
  Show help text and exit.

## COPYRIGHT
`gitaur` is Copyright (c) 2014 Vinson Chuong under The MIT License.

## SEE ALSO
makepkg(8), PKGBUILD(5)