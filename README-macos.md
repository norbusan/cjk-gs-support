External Database for cjk-gs-integrate
=============================================

Due to frequent incompatible changes in font file names by Apple,
the built-in database in cjk-gs-integrate doesn't support
OS X 10.11 El Capitan or later versions. Support for these
releases are provided in additional databases included in the
current package.

Usage
-----

Either install `cjk-gs-integrate-macos` from 
[TLContrib](https://contrib.texlive.info) or download the 
required database files directly from the 
[github account](https://github.com/texjporg/cjk-gs-support).

We provide the following additional databases:

- for El Capitan (10.11): [cjk-gs-integrate-elcapitan.dat](https://raw.githubusercontent.com/texjporg/cjk-gs-support/master/cjk-gs-integrate-elcapitan.dat)
- for Sierra (10.12): [cjk-gs-integrate-sierra.dat](https://raw.githubusercontent.com/texjporg/cjk-gs-support/master/cjk-gs-integrate-sierra.dat)
- for High Sierra (10.13): [cjk-gs-integrate-highsierra.dat](https://raw.githubusercontent.com/texjporg/cjk-gs-support/master/cjk-gs-integrate-highsierra.dat)

Download the database file (`*.dat`) which is suitable for
your OS version. Either place it in the current working directory
or into the directory `$TEXMF/fonts/misc/cjk-gs-integrate` where
`$TEXMF` is one of the TEXMF trees/

Then execute the script in the usual way (see main documentation) and add
the option `--fontdef-add`. For macOS 10.13 High Sierra this would be:

`````
[shell] cjk-gs-integrate[.pl] --fontdef-add=cjk-gs-integrate-highsierra.dat
`````

For OS X 10.11 El Capitan, use `cjk-gs-integrate-elcapitan.dat`.
For macOS 10.12 Sierra, use `cjk-gs-integrate-sierra.dat`.

Authors, Contributors, and Copyright
------------------------------------

Maintained by Japanese TeX Development Community. For development, see
  https://github.com/texjporg/cjk-gs-support

The script is licensed under GNU General Public License Version 3 or later.
The contained font data is not copyrightable.