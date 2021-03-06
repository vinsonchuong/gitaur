# gitaur
A set of command-line scripts that automate common tasks in maintaining
[AUR](https://aur.archlinux.org/) packages on GitHub.

## Scripts
* `gitaur-pkgbuild` populates an incomplete `PKGBUILD` with values derived
  from the corresponding GitHub repository and AUR deployment
  ([docs](doc/gitaur-pkgbuild.md), [code](bin/gitaur-pkgbuild)) 
* `gitaur-install` builds and installs a package
  ([docs](doc/gitaur-install.md), [code](bin/gitaur-install)) 
* `gitaur-publish` packages and uploads a GitHub project to the AUR
  ([docs](doc/gitaur-publish.md), [code](bin/gitaur-publish)) 

## Installing
`gitaur` is available as an
[AUR package](https://aur.archlinux.org/packages/gitaur/).
