# FlightAdvisor
FlightAdvisor is a single-file HTML dashboard that tells drone pilots whether it's safe to fly at a map-pin location. You pick a drone (any DJI model, or a micro FPV/Betaflight quad like the Flywoo Firefly 18 O4), then drop a pin on the map or search for a place.

It checks live weather from Open-Meteo against that aircraft's limits: wind, gusts, temperature, humidity, precipitation, rain within 5 miles, visibility and daylight. A separate airspace card uses FAA data for the pinned location: UAS Facility Map grid cell, altitude ceiling and military restrictions, plus your planned altitude (default 400 ft). The final recommendation combines weather and airspace into green, yellow or red. It also shows a 24-hour forecast strip, a dark/light theme toggle, and remembers your last drone and location.

It's advisory only. It doesn't check TFRs, NOTAMs, parks or local laws, and the FPV wind limits are estimates.

#### Created with Claude Sonnet 5.5
