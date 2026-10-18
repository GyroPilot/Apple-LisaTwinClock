# LisaTwinClock

Sets the Apple Lisa's clock to today's date. The Lisa's clock only counts the years 1981 to 1995, so LisaTwinClock
uses a **twin year**: a year in that range with the same calendar as this one (2026 becomes 1987), so every date
falls on the right weekday. The real year is kept in TWINYEAR.DATA beside the tool so tools can show true dates.

Tool number **419313** in the GyroPilot series. Lisa Pascal, Workshop 3.0, Lisa Office System 3.1.

## Status

- **1.0** -- set by hand. Tested on a LisaFPGA and a Lisa 2/10 (`releases/LISATWINCLOCK_1_0.dc42`).
- **1.1** -- also sets the clock from the network through an RS-232 FujiNet. Built and tested in LisaEm; waiting for
  its check on the 2/10 (`releases/LISATWINCLOCK_1_1_TEST.dc42`). The sources here are 1.1 (REV D).

## Using it

| Key | What it does |
|---|---|
| S | set the clock by hand: year, month, day, hour, minute (RETURN takes the value shown) |
| N | set it from the network: shows the network time and the twin-year date; Y sets the clock |
| C | show the clock and the real date |
| T, H | about twin years; help |

The **Network** menu picks where the time comes from: the FujiNet's own clock (in the time zone set on the FujiNet),
the web for your town (timeapi.io; your town is the one LisaFuji keeps in HOMETOWN.DATA on the same disk), or the web
for a time zone you type (America/New_York, Europe/London ...); and the speed, 9600 or 19200. Kept in TWCNET.DATA.

The Lisa 2/10 has no clock battery by design: it keeps time while plugged in and loses it when unplugged. Set the
clock after every power cut -- with a FujiNet, one key.

## Credits

Tim O'Connor (bmwcyclist on LisaList2, GyroPilot on GitHub), with Claude (Anthropic). Lisa Pascal with the Lisa
Workshop 3.0 for Lisa Office System 3.1; built in LisaEm and proven on a Lisa 2/10 and a LisaFPGA with a FutureVision
Research FujiNet for RS-232.
