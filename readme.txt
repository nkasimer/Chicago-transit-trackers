Chicago has several different transit APIs, which each have different syntaxes.
The CTA bus and train trackers are well documented, but the Divvy Bike API is poorly documented.
PACE buses have no official API, but data can be pulled from their bus tracker.

I thought it would be helpful to have a repo with different scripts for pulling Chicago-area transit APIs.
My intent is to help people who want to use those APIs by giving a starting point for code that pulls the APIs and turns them into useful output.

Traintracker pulls the CTA L API and turns it into a human-readable departure list given station IDs.
Bustracker does the same for the CTA and PACE bus APIs. Pulling the PACE bus tracking data is non-obvious and not documented, so that pull may be useful even without the human-readable bit.  The input required for PACE is a bit more involved than what's needed for the CTA API.
Divvyinfo pulls data on Divvy bikeshare, both nearby stations and nearby dockless bikes, for a given location.
Transfercalculator calculates transfers between CTA routes (train or bus) to output machine-readable data on a departure + departures that connect with that departure, and then turns that into human readable output.

The CTA's APIs require API keys, which can be obtained from the following links:
https://www.transitchicago.com/developers/bustracker/
https://www.transitchicago.com/developers/ttdocs/
These links also contain documentation for each of these APIs.