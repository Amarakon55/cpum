DCPU - Dmenu Central Processing Unit
================

## Contents

-   [Usage](#usage)
-   [Dependencies](#dependencies)
-   [Installation](#installation)
    -   [Universal](#universal)
    -   [Gentoo](#gentoo)
-   [Uninstallation](#uninstallation)
    -   [Universal](#universal-1)
    -   [Gentoo](#gentoo-1)

DCPU is a simple Dmenu script that allows you to manage your CPU
settings. It allows you to change:

1.  governor
2.  frequency
3.  minimum frequency
4.  maximum frequency

## Usage

``` sh
`# root` dcpu # launch the program and manage between options
`# user` dcpu --help # see available options
`# root` dcpu <option> # choose an option before launching the program
```

## Dependencies

1.  Dmenu
2.  cpupower

## Installation

### Universal

``` sh
`# user` git clone https://github.com/amarakon/dcpu
`# user` cd dcpu
`# root` make install
```

### Gentoo

``` sh
`# root` eselect repository add amarlay git https://github.com/amarakon/amarlay
`# root` emerge --sync amarlay
`# root` emerge x11-misc/dcpu
```

## Uninstallation

### Universal

``` sh
`# user` cd dcpu
`# root` make uninstall
```

### Gentoo

``` sh
`# root` emerge -c x11-misc/dcpu
# Remove my overlay (optional)
`# root` eselect-repository remove -f amarlay
`# root` emerge --sync
```
