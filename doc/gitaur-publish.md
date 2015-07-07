# gitaur-publish(1) -- populates and publishes a PKGBUILD to the AUR

## SYNOPSIS
`gitaur-publish` [_PKGBUILD_]<br>
`gitaur-publish` `-h`|`--help`<br>

## DESCRIPTION
`gitaur-publish` runs `gitaur-pkgbuild` to populate the `PKGBUILD` if it is
incomplete, creates a source package, and publishes it to the AUR.

If the path to a `PKGBUILD` is not provided, `gitaur-publish` will look in the
current working directory for a `PKGBUILD`.

`namcap` is used to check the generated `PKGBUILD` for any problems.

`mksrcinfo` (from the `pkgbuild-introspection` package) is used to build the
source package.

Note that the generated package will be published via Git to
`ssh://aur@aur4.archlinux.org/package`. `gitaur-publish` assumes that the SSH
key is in place to enable this action.

## OPTIONS
* -h, --help:
  Show help text and exit.

## COPYRIGHT
`gitaur` is Copyright (c) 2015 Vinson Chuong under The MIT License.

## SEE ALSO
gitaur-pkgbuild(1), namcap(1)
