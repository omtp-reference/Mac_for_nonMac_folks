# OSX/MacOS Install Errata

#### MacOS release date blocks older versions

Various Versions of macOS/OSX will fail to install for various reasons.
You can fix the worst of these by disconnecting from your wifi/ethernet and resetting
your NVRAM.  Then boot from your USB installer, open a terminal (from the Utilities menu) and type the following:
`date ##########` where the # numbers are listed below.  Format is: `MMDDhhmmYY`

| MacOS version | version name  | terminal date command                     |
| ------------- | ------------- | ----------------------------------------- |
| 13.x          | Ventura       | `date 0101010123` <- Currently not needed |
| 12.x          | Monterey      | `date 0101010122` <- Currently not needed |
| 11.x          | Big Sur       | `date 0101010121` <- Currently not needed |
| 10.15         | Catalina      | `date 0101010120` <- Currently not needed |
| 10.14         | Mojave        | `date 0101010119`                         |
| 10.13         | High Sierra   | `date 0101010118`                         |
| 10.12         | Sierra        | `date 0101010117`                         |
| 10.11         | El Capitan    | `date 0101010116`                         |
| 10.10         | Yosemite      | `date 0101010115`                         |
| 10.9          | Mavericks     | `date 0101010114`                         |
| 10.8          | Mountain Lion | `date 0101010113`                         |
| 10.7          | Lion          | `date 0101010111`                         |
| 10.6          | Snow Leopard  | `date 0101010110`                         |
| 10.5          | Leopard       | `date 0101010108`                         |

#### Create MacOS USB installer terminal commands

Note: These commands all assume that your MacOS installer is in your `/Applications` folder and that your target USB drive is named `Untitled`; adjust as necessary for your situation.
For macOS Catalina:
<code>sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled</code>
For macOS Mojave:
<code>sudo /Applications/Install\ macOS\ Mojave.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled</code>
For macOS High Sierra:
<code>sudo /Applications/Install\ macOS\ High\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled</code>
For OS X El Capitan
<code>sudo /Applications/Install\ OS\ X\ El\ Capitan.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled --applicationpath /Applications/Install\ OS\ X\ El\ Capitan.app</code>
For OS X Yosemite:
<code>sudo /Applications/Install\ OS\ X\ Yosemite.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled --applicationpath /Applications/Install\ OS\ X\ Yosemite.app --nointeraction</code>
For OS X Mavericks:
<code>sudo /Applications/Install\ OS\ X\ Mavericks.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled --applicationpath /Applications/Install\ OS\ X\ Mavericks.app --nointeraction</code>
