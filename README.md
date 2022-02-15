# DCPU – Dmenu Central Processing Unit

DCPU is a simple dmenu script that allows you to manage your CPU settings.
The usage is very simple:
* `$ dcpu` – launch the program and manage between options
* `$ dcpu <option>` – choose an option before launching the program

## Dependencies
1. cpu-cli

## (Un)Installation
### Universal
#### Installation
##### Latest Git Master (Bleeding Edge)
1. Git clone the repository.
* `$ git clone https://github.com/Amarakon55/dcpu`
2. Change working directory to *dcpu*.
* `$ cd dcpu`
3. Install DCPU using the Makefile
* `# make install`
#### Uninstallation
##### Latest Git Master (Bleeding Edge)
1. Change working directory to *dcpu*.
* `$ cd dcpu`
2. Uninstall DCPU using the Makefile
* `# make uninstall`

### Gentoo
#### Installation
##### Latest Git Master (Bleeding Edge)
1. Add my personal [Gentoo overlay](https://github.com/Amarakon55/amarlay) using [eselect-repository](https://packages.gentoo.org/packages/app-eselect/eselect-repository)
* `# eselect repository add amarlay git https://github.com/Amarakon55/amarlay`
2. Sync my personal [Gentoo overlay](https://github.com/Amarakon55/amarlay) using `emerge`
* `# emerge --sync amarlay`
3. Emerge the DCPU package
* `# emerge x11-misc/dcpu` or `# emerge dcpu`
#### Uninstallation
##### Latest Git Master (Bleeding Edge)
1. Unmerge the DCPU package
* `# emerge -c x11-misc/dcpu` or `# emerge -c dcpu`
2. (Optional) Remove my overlay
* `# eselect-repository remove -f amarlay`
3. (Optional) Sync using `emerge`
* `# emerge --sync`
