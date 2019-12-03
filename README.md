# Tally Marks

*Tally Marks* is a special-purpose OpenType font that is based on the Adobe-Identity-0 ROS (*ROS* stands for /Registry, /Ordering, and /Supplement, and refers to the /CIDSystemInfo dictionary entries that define the glyph set name for CID-based character collections). The Adobe-Identity-0 ROS is a special-purpose character collection whose use is not tied to a specific language.

Tally Marks is an OpenType-SVG font that primary includes glyphs for tally marks. The characters for two tally mark systems were added in [Unicode Version 11.0](https://www.unicode.org/versions/Unicode11.0.0/). One system is ideographic, and includes the following five characters in the [Counting Rod Numerals](https://www.unicode.org/charts/PDF/U1D360.pdf) block: U+1D372 &#x1D372; IDEOGRAPHIC TALLY MARK ONE, U+1D373 &#x1D373; IDEOGRAPHIC TALLY MARK TWO, U+1D374 &#x1D374; IDEOGRAPHIC TALLY MARK THREE, U+1D375 &#x1D375; IDEOGRAPHIC TALLY MARK FOUR &amp; U+1D376 &#x1D376; IDEOGRAPHIC TALLY MARK FIVE. The other system is Western, and includes the following two characters in the same block: U+1D377 &#x1D377; TALLY MARK ONE &amp; U+1D378 &#x1D378; TALLY MARK FIVE.

Glyphs for U+0020 &#x0020; SPACE, U+3000 &#x3000; IDEOGRAPHIC SPACE, and U+6B63 &#x6B63; (confusable with U+1D376 &#x1D376; IDEOGRAPHIC TALLY MARK FIVE), along with glyphs that represent the digits two through four in the Western tally mark system, are also included. The latter glyphs are accessible in apps that support the &#x0027;[ccmp](https://docs.microsoft.com/en-us/typography/opentype/spec/features_ae#ccmp)&#x0027; (*Glyph Composition/Decomposition*) GSUB feature, and sequences of two through five instances of U+1D377 &#x1D377; TALLY MARK ONE form the digits two through five. Yes, a sequence of five instances of U+1D377 &#x1D377; TALLY MARK ONE will form the glyph for U+1D378 &#x1D378; TALLY MARK FIVE.

In the [latest release](https://github.com/adobe-fonts/tally-marks/releases/latest) of this project you will find the ready-to-install OpenType-SVG font.

Note that some apps do not yet support OpenType-SVG fonts, in which case the glyphs for the tally marks simply appear in Black&amp;White. If the glyphs for tally marks appear in red (#FF0000), then the app supports OpenType-SVG fonts. The named &#x0027;[ss01](https://docs.microsoft.com/en-us/typography/opentype/spec/features_pt#tag-ss01---ss20)&#x0027; (*Stylistic Set 1*: *Black and White*) GSUB feature can be used to explicitly specify the Black&amp;White glyphs in environments that support OpenType-SVG fonts.

## Font installation instructions

* [macOS](https://support.apple.com/en-us/HT201749)
* [Windows](https://www.microsoft.com/en-us/Typography/TrueTypeInstall.aspx)
* [Linux/Unix-based systems](https://github.com/adobe-fonts/source-code-pro/issues/17#issuecomment-8967116)

## Building the font from source

### Requirements

To build the binary font file from source, you need to have installed the [Adobe Font Development Kit for OpenType](https://github.com/adobe-type-tools/afdko/) (AFDKO). The AFDKO tools are widely used for font development today, and are part of most font editor applications.

In order to add the [SVG](https://docs.microsoft.com/en-us/typography/opentype/spec/svg) (*Scalable Vector Graphics*) table, you will need to either install [*addSVGtable.py*](https://github.com/adobe-type-tools/opentype-svg) or [fonttools](https://github.com/fonttools/fonttools), depending on which method you use, both of which are described in the COMMANDS.txt file.

### Building the font

In this repository, all necessary files are in place for building the OpenType-SVG font, and the COMMANDS.txt file provides the command lines that are used.

## Getting Involved

For any suggestions for changes, please [create a new issue](https://github.com/adobe-fonts/tally-marks/issues) for consideration.

