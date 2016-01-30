# KeeTrayTOTP
Fork of the Tray TOTP Plugin for KeePass2.

Original work developed by the [Morphlin](http://sourceforge.net/u/morphlin/profile/) the source code and plugin can be found at http://sourceforge.net/projects/traytotp-kp2/

Most of consumer TOTPs use the RFC6238 output style, sadly some companies (eg.: Valve) decided not to adehere to the standard and instead build it's own format.

In the case of Steam Mobile Authenticator the new output format was reverse engineered by various developers, and alternatives to it starting to popping around, most to prety goodjob and can by themselves recover the TOTP secret (which is no easy task given Valve's implementation).

This plugin is for those who already use [Tray TOTP Plugin](http://sourceforge.net/projects/traytotp-kp2/), but also want to use with Valve's Steam.

## Dependencies
* [Keepass 2.31](http://keepass.info/)
* .NET 3.5 or superior

## So, why do this? 
Variou reasons, first and most important: I don't want to use another application only for steam! KeePass and Tray TOTP (with some modifications) are more than capable enough to handle this task.

Second: for education, working with another developer's code , specially in a language you're not familiar with, its a difficult task but not  uncommon situation.

### Steam TOTP Secret?!
There is no easy way to get it, there various complications. Since Steam doesn't setup like most services (using QR Codes), the easiest way is to have through a rooted android phone.

Another way would be using totp generators that support Steam like [Windows Authenticator](https://github.com/winauth/winauth) and [Steam Desktop Authenticator](https://github.com/Jessecar96/SteamDesktopAuthenticator), as far as I know, they emulate the mobile app API calls in order to generate a new TOTP Secret, one could use them to obtain the secret (never tried though), also this have the drawback of disabling the mobile app.

TODO: Tutorial how to get Steam TOTP secret

### What's next?
My first objective is complete: I made a working prototype.
But I'm not happy with the code, I want to rebuild this thing from the ground if needed, I'm by no means criticizing the original work, but it's little complex for me and rebuilding it may help to better understanding it. 
Also I'm open to suggestion, issues, new features, etc.


**Thanks to [Dominik Reichl](http://www.dominik-reichl.de/) for KeePass software and to [Morphlin](http://sourceforge.net/u/morphlin/profile/) for the original plugin**

English isn't my native language, so please excuse any mistakes.
