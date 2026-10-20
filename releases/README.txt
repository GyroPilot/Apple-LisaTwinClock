LisaTwinClock 1.1 for the Apple Lisa Office System       October 2026 (release build REV E)
Sets the Lisa's clock to today's date, in the twin year.  Tool 419313.

WHY
  The Lisa's clock only counts 1981 to 1995.  LisaTwinClock sets it to the year in that range
  with the same calendar as today, so every date lands on the right weekday: 2026 becomes 1987.
  The real year is saved in TWINYEAR.DATA beside the tool, so LisaTwinClock (and LisaFuji) can
  show the true date.

USE
  Open it: the first screen shows the Lisa's clock and, if the note exists, the real date.
    S   set the clock: type today's date and time (the twin year is worked out for you).
    C   show the clock and the real date.
    T   twin-year table.      H   help.      About shows the version.
    N   NEW: set the clock from the network, with an RS-232 FujiNet on Serial B.  The Network
        menu chooses where the time comes from:
          the FujiNet's own clock (the time zone set on the FujiNet), or
          the web for your town (timeapi.io, summer time included; your town is the one
          LisaFuji keeps in HOMETOWN.DATA on the same disk), or
          the web for a time zone you type, such as America/New_York or Europe/London.
        and the speed (9600 or 19200).  The choice is kept in TWCNET.DATA.  You see the
        network time and the twin-year date first; Y sets the clock.
  Apple's own Clock tool will then agree.  LisaFuji's C does the same set from the network.

NOTES
  The Lisa 2/10 has no clock battery, by design: it keeps the clock while plugged in (even
  switched off at the button) and loses it whenever it is unplugged.  Only the Lisa 1 and 2/5
  had batteries, and most of those have since leaked.  So on a 2/10, set the clock after
  every power cut; LisaFuji's C does it from the network in one key.  Nothing is changed without pressing S or Y.
  Typing at a prompt redraws only the line you type on (no flicker on a real Lisa).
  Known: when a new screen opens (for example the Network options) the window is redrawn, so it may
  refresh for a moment.  Typing itself does not flash.

SOURCE
  Lisa Pascal, Workshop 3.0.  github.com/GyroPilot/LisaTwinClock
  Tim O'Connor (bmwcyclist), with Claude.  Tested on a LisaFPGA and a Lisa 2/10, October 2026.

WHAT'S IN THIS RELEASE
  LISATWINCLOCK_1_1.dc42         the release floppy
  LisaTwinClock_1.1_source.zip   Lisa Pascal sources and exec files (with LisaFuji's FnBus unit)
  About says "LisaTwinClock 1.1 (20 October 2026)".
