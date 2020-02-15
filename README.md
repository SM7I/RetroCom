# RetroCom
RetroCom information and the Client / Server software suite for ZX Spectrum, Sinclair QL, Sinclair ZX81 & Commodore 128.

Timeframe for release on different platforms:
* ZX Spectrum - Done
* Sinclair QL - Q1 20
* ZX81 - Q1 20
* Commodore 128 - Q1 20
* Amiga - TBD
* Commodore 64 - TBD
* Atari ST - TBD

**Consider this as a pre-release as of now**

RetroCom is an hardware interface, which I build, that allows retro computers access to the Internet by the means of WiFi to your local network. The interface takes AT commands according to the manual of Zimodem, however I've modified the firmware and added own commands, such as AT+PING.

Even though this is a functional way to communicate with services on the Internet I decided to develop a software suite for the interface. The software suite is written in portable C thus allowing the same source code for different platforms.

The suite consists of two parts, one server part and one client part. The server part runs on either Linux or Windows (with root / admnistrator equivalent rights) as a daemon listening om TCP port 2323 for client connections.

The client part is available for the following retro computers at the moment (more will follow):

* ZX Spectrum 128K (TAP file)
* ZX Spectrum 48K equipped with IF1 (TAP file)

As for now there are some limitations in functionality due to technical reasons being solved while this is written, Upload and Download of data to / from server does not work, but will resolved as quickly as possible.

**Quick guide of keys:**

W = connect to Wifi SSID (syntax: SSID, password)

S = connect to server (syntax: IP or hostname:2323 (of course you can also connect to IRC servers, in that case port needs to be 6667))

F = List server side files

D = Download (not working atm)

U = Upload (not working atm)

P = Ping IP or hostname

B = Disconnect from server

M = Extended menu (not implemented atm)

A = About
