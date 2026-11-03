# LisaTwinClock changelog

## 1.3 update 1 (REV L) -- 3 Nov 2026 -- RELEASE (tested on the 2/10, 3 Nov)
- N through an ESProFile uses the ESProFile (on a 2/10 it had fallen back to Serial B).
- It looks for the mailbox as "ESPFuji Mailbox" first, then MAILBOX.DATA, so old setups keep working.
- A damaged TWINYEAR.DATA no longer blocks the note: it is remade, or kept in TWINYEAR2.DATA, and the newer good one
  is read.
- A failed connection through an ESProFile now shows the ESProFile's own reason ("the drive said: ...") instead of
  only "status 207".
- The Version box names the ESProFile route.
## 1.3 REV H -- 30 Oct 2026 -- RELEASE
- FnBus at LisaFuji's REV Z level: the ESPFuji ESProFile mailbox as a third source of the time (FnSetVol + FnMbUp at
  launch; the source line says "the ESProFile's clock" and no baud rate on that route). Version box: 1.3, 30 October.
  Tim, 30 Oct: every app follows a hardware change.
## 1.2 REV F / REV G -- 22-23 Oct 2026 -- RELEASE (staged)
- The Network menu's Use 9600 / Use 19200 baud sets the FujiNet too (its web page through the N: device, then its
  Reset button, then the port again at the new speed); the first port open of each launch probes for the speed and
  keeps what answers (FnFind). FnBus brought to LisaFuji's REV S level (Serial A or B ready, FnSetBd, FnFind).
  REV G = REV F with the version shown as 1.2. LisaEm-tested the night of 22 Oct.
## 1.1 REV E -- 20 Oct 2026 -- RELEASE BUILD (staged, not published)
- Typing at a prompt redraws only the line you type on (no flicker on a real Lisa).
- About says 20 October 2026; the floppy's disk name is 'LisaTwinClock 1.1' (it said 0.1).
- Opened from its floppy in LisaEm.  Tim decides when to publish.
- Known: when a new screen opens (for example the Network options) the window redraws and may refresh for a moment.
- Typing at a prompt was checked on a Lisa 2/10 on 20 Oct 2026: no flashing.
## 1.1 REV D -- 17 Oct 2026 -- built, waiting for the 2/10
- N and the Network menu: the time from the FujiNet's clock, or from timeapi.io for your town or a typed time zone;
  9600 or 19200 baud; the choice kept in TWCNET.DATA.
## 1.0 REV C -- 17 Oct 2026 -- RELEASE 1.0
- The version shown as 1.0.
## 0.1 REV A-B -- 10-16 Oct 2026
- First build: set the clock by hand to the twin year, read it back, keep the real year in TWINYEAR.DATA.
