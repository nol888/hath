# hath

Make sure to read and understand the license for this program, found in the file LICENSE or at http://www.gnu.org/licenses/gpl.txt, before you start playing with it.

## Changes with respect to vanilla hath

 - Monitor active requests via GUI. (not sure if this still works)
 - It's on GitHub! (yay FoSS)

## Coming soon

 - Maven???
 - Serve an index of the cache directory?????
 - Unit????tests???

## Building

In order to build Hentai@Home, you need the following:
  - The sqlite-jdbc-3.7.2 SQLiteJDBC library, placed in this directory (obtainable from http://g.e-hentai.org/hentaiathome.php or http://www.xerial.org/trac/Xerial/wiki/SQLiteJDBC)
  - The Java(TM) SE JDK, version 6 or greater

In a Windows build environment, run make.bat and makejar.bat in order. On Linux, do make then make jar (or make all). This will produce two .jar files, HentaiAtHome.jar and HentaiAtHomeGUI.jar, in the current directory. These two files along with sqlite-jdbc-3.7.2 constitutes the entire program.

Move the three .jar files to a location of your choice (this is where H@H will store all its files), and run java -jar HentaiAtHome.jar for the CLI version or java -jar HentaiAtHomeGUI.jar for the GUI version.

## Notes

Note that this package only contains the Hentai@Home Client, which is coded specifically for E-Hentai Galleries. The server-side systems are highly dependent on the setup of a given site, and must be coded specially if it's to be used for other sites.
