Keymapper v0.1
==

Keymapper is a portable tool to remap the Caps Lock key to the [Chrome App Launcher for Windows](http://blog.chromium.org/2013/02/chrome-app-launcher-developer-preview.html) without rebooting on Windows®.

By remapping the Caps Lock to the Chrome App Launcher, the behavior is more like on ChromeOS and Chromebooks.
	
How it Works
--

Caps Lock keypresses are intercepted with a global keyboard hook (SetWindowsHookEx). Chrome App Launcher is invoked via a ShellExecute command.

Known Issues
--

Certain anti-virus heuristics may classify the executable as a potential threat due to the keylogging potential of a global keyboard hook. A more permanent way to remap your keyboard is using a registry tool like SharpKeys.