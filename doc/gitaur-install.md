# gitaur-install(1) -- populates and installs a PKGBUILD

## SYNOPSIS
`gitaur-install` [_PKGBUILD_]<br>
`gitaur-install` `-h`|`--help`<br>

## DESCRIPTION
`gitaur-install` runs `gitaur-pkgbuild` to populate the `PKGBUILD` if it is
incomplete, creates a package, and installs it. This is useful in testing a
package locally before deploying it to the AUR.

If the path to a `PKGBUILD` is not provided, `gitaur-install` will look in the
current working directory for a `PKGBUILD`.

`namcap` is used to check the generated `PKGBUILD` for any problems.

`makepkg` is used to build the package.

## OPTIONS
* -h, --help:
  Show help text and exit.

## COPYRIGHT
`gitaur` is Copyright (c) 2015 Vinson Chuong under The MIT License.

## SEE ALSO
gitaur-pkgbuild(1), makepkg(8), namcap(1)
