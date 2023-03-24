# I_AM_ROOT_patches
A set of patches for common unix programs to disable 'don't run me as root' checks. Laid out in a format to allow being cloned into portage/patches on Gentoo.  
Note: possibly bad idea. your own risk yadda yadda. you know what you're doing already, or you wouldn't be here :)  

I doubt any changes I make here are 'copyrightable', but if it makes you happy, any copyrightable additions I make here are dual licensed under both 0-clause-BSD + MIT. Go ham.

## Patches:
sway: allows running as root and also re enabled the SUID functionality. WIP support for not needing seatd.  
wlroots: without this, wlroots starts an X server that non-root users can't connect to.  
steam: steam has a built in check to disable running as root in shell. disabled. also a forked .desktop file as it needs the CEF sandbox removed to run as root.  
postgres: disables the anti-run-as-root check, but does not disable behavior like the same user needing to own the database, yadda yadda.  
