# Font-Validator

Font Validator is a tool for testing fonts prior to release. 
It was initially developed by Microsoft, to ensure that fonts meet Microsoft's high quality standards and perform exceptionally well on Microsoft's platform.

In 2015 the source code was published under the MIT license ([see release discussion](http://typedrawers.com/discussion/1222/microsoft-font-validator-lives))

## Usage

`FontVal.exe` is the GUI, and `FontValidator.exe` shows usage and example if run without arguments; both should be self-explanatory. 
We provide all-in-one native command-line binaries, `FontValidator`, for Mac OS X and Linux, as of Release 2.1.1.
Georg Seifert contributed a friendly GUI wrapper for Mac around the command-line tool.

The GUI's built-in help requires a CHM viewer, which defaults to [chmsee](https://github.com/jungleji/chmsee) on GNU+Linux, or via env variable `MONO_HELP_VIEWER` 

The GUI on X11/mono needs the env variable `MONO_WINFORMS_XIM_STYLE=disabled` set to work around [Bug 28047 - Forms on separare threads -- Fatal errors/crashes](https://bugzilla.xamarin.com/show_bug.cgi?id=28047)

## Binary Downloads

Since Release 2.0, binaries (`*.dmg` for Mac OS X, `*-bin-net2.zip` or `*-bin-net4.zip` for MS .NET/mono) are available from
[Binary Downloads](https://sourceforge.net/projects/hp-pxl-jetready/files/Microsoft%20Font%20Validator/).
From Release 2.1 onwards, gpg-signed binaries for Ubuntu Linux are also available. There is an additional and simplified location for
Binary downloads at the [Releases link above this page](https://github.com/HinTak/Font-Validator/releases).

Please consider [donating to the effort](https://sourceforge.net/p/hp-pxl-jetready/donate/), if you use the binaries.

[Build Instructions](https://github.com/HinTak/Font-Validator/wiki/Build-Instructions)

### Status

[The FontVal 2.2 Roadmap](https://github.com/HinTak/Font-Validator/wiki/Two-years-on,-and-2.2-Roadmap).

As of Release 2.0 (July 18 2016), all the withheld parts not released by Microsoft were re-implemented.
Release 2.0 run well on non-windows, and is substantially faster also.
Existing users of the increasingly dated 1.0 release from 2003 are encouraged to upgrade.
There are a number of known disagreements and issues which are gradually being filed and addressed.
[README-hybrid.txt](README-hybrid.txt) is now of historical interests only.

Release 2.1 is considered to fully supercede the proprietary 1.0 feature-wise and functionality-wise.

* The DSIG test (DSIG_VerifySignature) does not validate trusted certificate chain yet.

* Many post-2nd (i.e. 2009) edition changes, such as CBLC/CBDT and other new tables.

* Very few post-3rd (i.e. 2015) edition changes are implemented.

See also [README-extra.txt](README-extra.txt) for a list of other interesting or non-essential tasks.

