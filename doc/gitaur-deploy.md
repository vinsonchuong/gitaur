# gitaur-deploy(1) -- populates and deploys a PKGBUILD to the AUR

## SYNOPSIS
`gitaur-deploy` <PKGBUILD><br>
`gitaur-deploy` `-u` <username> `-p` <password> [`--`] <PKGBUILD>...<br>
`gitaur-deploy` `-h`|`--help`<br>

## DESCRIPTION
`gitaur-deploy` runs `gitaur-pkgbuild` to populate the `PKGBUILD` if it is
incomplete, creates a source package, and uploads it to the AUR.

`namcap` is used to check the generated `PKGBUILD` for any problems.

`mkaurball` (from the `pkgbuild-introspection` package) is used to build the
source package.

`burp` is used to upload the source package to the AUR.

If a username and password are not given, `burp` will prompt for them.

## OPTIONS
* -h, --help:
  Show help text and exit.
* -u, --user <username>:
  Upload the the AUR has the given user.
* -p, --pass <password>:
  Authenticate as the given user with the given password.

## COPYRIGHT
`gitaur` is Copyright (c) 2015 Vinson Chuong under The MIT License.

## SEE ALSO
burp(1), gitaur-pkgbuild(1), namcap(1)
