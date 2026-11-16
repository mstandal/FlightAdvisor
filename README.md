# FlightAdvisor
FlightAdvisor is a single-file HTML dashboard that tells drone pilots whether it's safe to fly at a map-pin location. You pick a drone (any DJI model, or a micro FPV/Betaflight quad like the Flywoo Firefly 18 O4), then drop a pin on the map or search for a place.

**Weather:** live Open-Meteo data is checked against that aircraft's limits: wind, gusts, temperature, humidity, precipitation, rain within 5 miles (no-go within 2.5 mi, caution at 2.5–5 mi for aircraft that aren't water-resistant), visibility and daylight. A 24-hour strip shows how conditions change.

**Airspace:** a separate card uses FAA data for the pinned location. It shows the UAS Facility Map grid cell, the altitude ceiling and national security restrictions. You enter a planned altitude (default 400 ft), and the card states which airspace class that altitude is in. A ground-to-ceiling diagram shows your altitude against the cell ceiling, with typical adjacent airspace above for reference.

**VFR chart:** the card also shows an FAA Sectional or Terminal Area chart snippet centered on the pin, with rings at 1 and 3 miles.

**Final recommendation:** the green/yellow/red call combines weather and airspace, whichever is worse, so good weather with an authorization requirement or an altitude above the cell ceiling shows yellow or red. The call also shows the weather and airspace verdicts separately.

It also has a dark/light theme toggle, remembers your last drone, location and planned altitude, and runs entirely in the browser with no server.

It's advisory only. It doesn't check TFRs, NOTAMs, parks or local laws automatically, the FPV wind limits are estimates, and the airspace layers above the grid ceiling are typical values, not FAA data.

#### Created with Claude Sonnet 5.5
