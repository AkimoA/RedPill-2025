# RedPill-2025

This is Red Pill, a 3D OpenGL "Matrix" screensaver for Mac OS X and macOS.
* Copyright © 2002-2012 mathew <meta@pobox.com>.
* Copyright © 2016 - px3 <rr@rdsroot.net>.
* Copyright © 2020 - Jason Short
* Copyright @ 2025 - AkimoA

Yes, this is a fork of a fork with a spoon :)
I updated to use current XCode and Mac OS formats (macOS 15 and XCode 16.4). 

Mostly I wanted this to run on my current machine which is a M2 which suffered from the legacyScreensaver-NoExitBug where the process would run indefinte after closing the screensaver and cloak up CPU/Memory. 
its build to support both arm64 and x86_64 .

Screensaver can't be opened?

Setting the screensaver and showing only black screen may be related to this issue. After unlocking from the black screen, it may show an alert like

Screensaver can’t be opened because Apple cannot check it for malicious software

Here is what you can do to solve it:

Open System Settings
Go to Privacy & Security
Scroll down to the bottom and click allow RedPill.saver to open anyway
Go back to Screen Saver in System Settings, and select Redpill as the screensaver
Click on "Open Anyway" when the alert pops up again

the ultimate goal would be to rewrite it in Swift / Metal

Red Pill is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
or visit [http://www.fsf.org/](http://www.fsf.org/)

