# knowledgejunkie-packaging-deps

## Description

A [Debian GNU/Linux][debian] metapackage to install a variety of tools and documentation used in
regular Debian packaging and packaging for the [Debian Perl][debian-perl] team.

Packages installed with this metapackage include:

- build-essential
- pkg-perl-tools
- packaging-dev
- cowbuilder
- dput
- myrepos
- equivs

- debian-policy
- developers-reference
- maint-guide
- debian-reference-en
- debian-faq
- debian-handbook
- debian-kernel-handbook
- debian-history


## Building the metapackage

A simple way to build the binary package is to change to the checkout directory and run:

    $ debuild -i -I -uc -us -b

This will generate the binary .deb file in the checkout's parent directory.

To clean the build directory afterwards, run:

    $ debuild clean


## Installing the metapackage

We can intall the local package using dpkg, and then install the missing dependencies using apt-get:

    # dpkg --install /path/to/knowledgejunkie-packaging-deps_0.x_all.deb
    # apt-get -f install


## License

GPL-2+


## Thanks

I hope you find this metapackage useful. Feel free to follow me on [GitHub][github] and [Twitter][twitter].

[debian]: http://www.debian.org/
[debian-perl]: https://pkg-perl.alioth.debian.org/
[github]: https://github.com/knowledgejunkie
[twitter]: http://twitter.com/nickmorrott
