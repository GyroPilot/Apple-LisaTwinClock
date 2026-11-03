LisaTwinClock 1.3, update 1 (3 November 2026, release build REV L)      tool 419313
Same LisaTwinClock 1.3 program with these changes, tested on a Lisa 2/10 through an ESProFile running ESPFuji
on 3 November 2026; the floppy LISATWINCLOCK_1_3.dc42 replaces the earlier one of the same name:
- N through an ESProFile uses the ESProFile (on a 2/10 it had fallen back to Serial B).
- It looks for the mailbox as "ESPFuji Mailbox" first, then MAILBOX.DATA, so old setups keep working.
- A damaged TWINYEAR.DATA no longer blocks the note: it is remade, or kept in TWINYEAR2.DATA, and the newer
  good one is read.
- A failed connection through an ESProFile now shows the ESProFile's own reason ("the drive said: ...")
  instead of only "status 207".
- The Version box names the ESProFile route.

--------------------------------------------------------------------------------------------------------------

LisaTwinClock 1.3 for the Apple Lisa Office System       30 October 2026 (release build REV H)
Sets the Lisa's clock to today's date, in the twin year.  Tool 419313.

New in this build: the time can come from an ESPFuji ESProFile (https://github.com/GyroPilot/ESPFuji) as well as an
RS-232 FujiNet or a LisaNet: put the tool on the ESProFile's volume and it finds the mailbox at launch, no serial
adapter.  Otherwise the 1.2 program.  Floppy image LISATWINCLOCK_1_3.dc42; the source zip has the Lisa Pascal sources
and the exec files.  Built with the Lisa Workshop 3.0 in LisaEm; the ESProFile route is the unit proven in LisaFuji 1.2
on a Lisa 2/10, not yet run with TwinClock itself on a Lisa.
