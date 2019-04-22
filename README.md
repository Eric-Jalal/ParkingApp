# ParkingApp

I wrote this code during a test assignment which the problem description was as written below:

## MAP INTERFACE FOR ANDROID

(1) Summary
- Single page application, Activity containing a full screen MapFragment
- For this task you need to obtain a Google Maps API key from Google

(2) Instructions
- As an attachment in this email there is a JSON object that contains map data for hypothetical
parking zones. This is dummy data snippet simulating a response received from the backend
system. Handle the data like it was the result received from the backend.
- Store/initialize the data in a way you feel is appropriate in this case. Among other things, each
of the zones have a polygon object, that consists of latitude/longitude coordinate pairs which
define the zone area.
- Load the map view (with the viewport based on location_data.bounds)
- Draw the zone polygons (location_data.zones.polygon) on top of the map. Use the
payment_is_allowed value for deciding the background color of the polygon.
- Draw a map pin in the center coordinate of the map. Customise the map pin so that it displays
the service price for the selected zone at the center of the pin (selected zone is explained later
on)
- Dragging/interacting the map changes the location of the map pin in a way, that once you stop
touch gestures (e.g. dragging) on the map, the map pin always appears at the center coordinate
of the map. While the map is being dragged, the pin should be hidden.
- Make a creative way of displaying other zone information (location_data.zones) for the
currently selected zone. Currently selected zone is the one where the map pin (current location)
is located (coordinate is within the zone polygon) and dragging the map pin into another zone
should select this zone. Once a zone is selected, the background color of the zone polygon also
changes.
- Place a "Start parking"-button as a part of your layout. Once tapped, the app will tell which
zone is being parked.

## Problems
- This code has a problem in polygon draweres which they are all connected together and it should not be like this, i have to fix it at some point.

## Disclaimer
This code published here is originally mine and is not allowed to be used by anybody for any purposes.


-
'# BSD 3-Clause License

Copyright (c) 2019, Amir Jalal
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its
   contributors may be used to endorse or promote products derived from
   this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.'
