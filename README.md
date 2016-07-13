Summon
======

<img src="mobile-app/res/icon-android.png" alt="Summon" height="80" align="left"><i>The browser for the Web of Things. </i>
<br />A platform for mobile devices that provides a convenient and scalable mechanism for IoT device interactivity, enabled by web-based interfaces and driven by the devices themselves.

<img src="https://lh3.googleusercontent.com/uDW2QXPCBx3a6gmGh_NUEPz7wNyMpDpMNhpvsXNyBa4VpbfWYqMauiGlVkAsOBWkzFY=h617"/>
<img src="https://lh3.googleusercontent.com/g9LttUc4AtQ0sbw3-9V9tnXXhUD8XrHybek4gvMi57jmeimFq9tlof4NVndA0dIOl-E=h617"/>

[<img src='https://play.google.com/intl/en_us/badges/images/generic/en-play-badge.png' alt="Google Play Store" height=38 />](https://play.google.com/store/apps/details?id=edu.umich.eecs.lab11.summon)
[<img src="http://images.apple.com/itunes/link/images/link-badge-appstore.png" alt="iOS App Store" height=40 />](https://itunes.apple.com/us/app/summon-lab11/id1051205682)

####Video
[![Video](http://img.youtube.com/vi/oQLkUcQoUe4/0.jpg)](https://youtu.be/oQLkUcQoUe4)

Peripherals
-----------

To quickly create a Bluetooth beacon device to test with, install the [Eddystone-URL app](https://play.google.com/store/apps/details?id=edu.umich.eecs.lab11.eddystone) on a separate Android device.

For Bluetooth peripherals to be listed in the Summon's scan, it must advertise the URI for its corresponding web interface according to the [Bluetooth URI AD type specification](https://www.bluetooth.org/DocMan/handlers/DownloadDoc.ashx?doc_id=302735) (page 27), or the [Eddystone-URL specification](https://github.com/google/eddystone/blob/master/protocol-specification.md).

Local Wi-Fi peripherals can advertise the URL as an HTTP service over mDNS/ZeroConf/Bonjour.

Example implementations of peripherals can be found in [`peripherals/examples/`](peripherals/examples).


Creating Interactive User Interfaces
------------------------------------

In addition to opening regular websites, Summon can open app-like web UIs that can make use of native smartphone features. These UIs are still developed using standard web tools, but they are able to do things like interact directly over Bluetooth and perform native application functions with provided Javascript APIs. Once the UI is hosted online or served locally from the device, the peripheral can advertise a link to it, as with an ordinary website.

Further details are in the [User Interfaces README](user-interfaces/README.md).
Example implementations of UIs can be found in [`user-interfaces/examples/`](user-interfaces/examples).
