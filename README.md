# fire-app-vpn

# Use at own risk 

Exploring vpn options on Fire TV/Stick

Enabling VPN Access in Fire TV


In response to how to capture network traffic posted in
https://stackoverflow.com/questions/38679188/capture-network-traffic-programmatically-no-root
one response pointed to
* Google's sample ToyVPN https://android.googlesource.com/platform/development/+/master/samples/ToyVpn
* based on which a full project was created at https://github.com/hexene/LocalVPN

This project explores creating a VPN app for Fire TV.

Updates after experiments:
* There are missing parts in the code. For e.g. PORT is not specified anywhere.
* ToyVPN GitHub code is here: https://github.com/aosp-mirror/platform_development/tree/master/samples/ToyVpn 
  * Client has interesting things such as SECRET and PORT
  * Server code for Linux is given. Porting this to OSX turned out to be hard. 
    * OSX has UTUN interfaces. Not sure how they can be used for this VPN service that support TCP and UDP protocols.
    * Not clear what impact of "up/down" states of UTUN are on the machine's security levels.
* After being able to see log files, I stopped working on this project. 

Result: Transmission of packets through VpnService has <b>NOT</b> been tested.
  




