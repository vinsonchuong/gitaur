# gitaur
A set of command-line scripts that automate common tasks in maintaining
[AUR](https://aur.archlinux.org/) packages on GitHub.

## Scripts
* `gitaur-pkgbuild` populates an incomplete `PKGBUILD` with values derived
  from the corresponding GitHub repository and AUR deployment
  ([docs](docs/gitaur-pkgbuild.md), [code](bin/gitaur-pkgbuild)) 
* `gitaur-deploy` packages and uploads a GitHub project to the AUR
  ([docs](docs/gitaur-deploy.md), [code](bin/gitaur-deploy)) 

## Installing
`gitaur` is available as an
[AUR package](https://aur.archlinux.org/packages/gitaur/).
