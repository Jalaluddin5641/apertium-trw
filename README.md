Torwali

                            apertium-trw
===============================================================================

This is an Apertium monolingual language package for Torwali. What
you can use this language package for:

* Morphological analysis of Torwali
* Morphological generation of Torwali
* Part-of-speech tagging of Torwali

Requirements
===============================================================================

You will need the following software installed:

* lttoolbox (>= 3.3.0)
* apertium (>= 3.3.0)
* vislcg3 (>= 0.9.9.10297)
* hfst (>= 3.8.2)

If this does not make any sense, we recommend you look at: www.apertium.org

Compiling
===============================================================================

Given the requirements being installed, you should be able to just run:

$ ./configure
$ make

You can use ./autogen.sh instead of ./configure if you're compiling
from SVN.

If you're doing development, you don't have to install the data, you
can use it directly from this directory.

If you are installing this language package as a prerequisite for an
Apertium translation pair, then do (typically as root / with sudo):

# make install

You can give a --prefix to ./configure to install as a non-root user,
but make sure to use the same prefix when installing the translation
pair and any other language packages.

Testing
===============================================================================

If you are in the source directory after running make, the following
commands should work:

$  echo "TODO: test sentence" | apertium -d . trw-morph
TODO: test analysis result

$ echo "TODO: test sentence" | apertium -d . trw-tagger
TODO: test tagger result

Files and data
===============================================================================

* apertium-trw.trw.lexc          - Morphotactic dictionary
* apertium-trw.trw.twol          - Morphophonological rules
* apertium-trw.trw.rlx           - Constraint Grammar disambiguation rules
* apertium-trw.post-trw.dix      - Post-generator
* trw.prob                       - Tagger model
* modes.xml                      - Translation modes

For more information
===============================================================================

* http://wiki.apertium.org/wiki/Installation
* http://wiki.apertium.org/wiki/apertium-trw
* http://wiki.apertium.org/wiki/Using_an_lttoolbox_dictionary

Help and support
===============================================================================

If you need help using this language pair or data, you can contact:

* Mailing list: apertium-stuff@lists.sourceforge.net
* IRC: #apertium on irc.freenode.net

See also the file AUTHORS included in this distribution.

