# knowledgejunkie-packaging-deps

## Description

A [Debian GNU/Linux][debian] metapackage to install a variety of tools and documentation used in
regular Debian packaging and packaging for the [Debian Perl][debian-perl] team.

Packages installed with this metapackage include:

- build-essential
- cowbuilder
- debian-faq
- debian-handbook
- debian-history
- debian-kernel-handbook
- debian-policy
- debian-reference-en
- developers-reference
- dput
- equivs
- maint-guide
- myrepos
- packaging-dev
- pkg-perl-tools


## Building the metapackage

Build the binary package using git-buildpackge:

    $ gbp buildpackage

This will generate the binary .deb in gbp's configured output directory.


## Installing the metapackage

We can install the package using gdebi, which will automatically install
any missing dependencies

    # gdebi knowledgejunkie-packaging-deps_<version>_all.deb


## License

Copyright: 2016-20, Nick Morrott <nickm@debian.org>
License: GPL-2+


## Thanks

I hope you find this metapackage useful. Feel free to follow me on [GitHub][github] and [Twitter][twitter].

[debian]: http://www.debian.org/
[debian-perl]: https://pkg-perl.alioth.debian.org/
[github]: https://github.com/knowledgejunkie
[twitter]: http://twitter.com/nickmorrott
