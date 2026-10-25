# Code Table Generator – changelog

## v3.0 – 26 Oct 2026
- First GitHub Pages build. Version stamp now shown in the header.
- Ipswich: zone, precinct, local area, PIA, OV6 height/lot size, road hierarchy and OV1–OV15 overlays read live from ePlan through the Meliora relay. Falls back to ePlan direct, then says plainly that overlays were not checked.
- Relay failure rules: warns when the relay file is over 6 hours old; re-reads the relay once if ePlan rejects the token (498/499); cache-buster on every read. Flood comes from the five OV12 flood risk category layers (the combined layer is ignored).
- Wired to the mce-planning-rules skill: its engineering-code, Ipswich lot-type and Logan precinct constants are injected and checked on every build.
- Brisbane building work: demolition-only route, raising/repositioning (TBC demolition Section C), build-under via TBC design, small lots list the small lot house code instead of the zone code, heritage places switch the TBC codes off, front-setback 20% band calculator, extra QA notes (West End, Red Hill, Kedron lessons).
- DA Form 2 (building work) draft output.
