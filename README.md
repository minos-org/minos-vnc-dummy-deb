Debian packaging for minos-vnc-dummy
------------------------------------

Steps to build this package:

```
$ git clone --dept=1 https://github.com/minos-org/minos-vnc-dummy-deb
$ cd minos-vnc-dummy-deb
$ dch -i #insert proper upstream version (1:$(date +%Y%m%d%H%M)+git7digitsHash-minos)

[ Optional, make some adaptations, like updating debian/patches, if needed ]
[ document additional changes if required, $EDITOR debian/changelog ]

$ debuild -S

[ Build .dsc (pbuilder) || Upload .changes file (dput) ]
```
