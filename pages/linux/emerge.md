# emerge

> Gentoo Linux package manager utility.
> For equivalent commands in other package managers, see <https://wiki.archlinux.org/title/Pacman/Rosetta>.
> More information: <https://wiki.gentoo.org/wiki/Portage#emerge>.

- Synchronize all packages:

`sudo emerge --sync`

- Update all packages, including dependencies:

`sudo emerge {{-avuDN|--ask --verbose --update --deep --newuse}} @world`

- Resume a failed updated, skipping the failing package:

`sudo emerge --resume --skipfirst`

- Install a new package, with confirmation:

`sudo emerge {{-av|--ask --verbose}} {{package}}`

- Remove a package, its dependencies, and orphaned packages with confirmation:

`sudo emerge {{-avc|--ask --verbose --depclean}} {{package}}`

- Remove orphaned packages (that were installed only as dependencies):

`sudo emerge {{-avc|--ask --verbose --depclean}}`

- Search the package database for a keyword:

`emerge {{-S|--searchdesc}} {{keyword}}`
