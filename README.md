# Cernak Lab Interactive Instrument Map
[Live map](https://didwang.github.io/Cernak-lab-interactive-map/map-interface/)

This page shows an interactive floor map of the Cernak Lab with the location and status of major instruments.

## What you can do
See where each instrument is in the lab.

Check if an instrument is green (OK) or red (problem / attention needed).

Click an instrument to view:

1. Status
2. Steward
3. Last calibrated date
4. Next PM (preventive maintenance) due date
5. Links to the manual, log form, history log, and status sheet

**Red markers** blink so that issues are easy to spot at a glance.

## How to update status and maintenance info
All information comes from a shared Google Sheet.

1. Open the “CHANGE RED/GREEN” link from any instrument popup.
2. Update the Status, Steward, Last_Calibrated, or Next_PM_Due cells for that instrument.
3. Changes will appear on the map after a refresh (it may take a few seconds).
4. Status convention: green → instrument OK (solid green marker, no blinking); Anything else → treated as red (blinking red marker).

## How to add a log entry
Use the “ADD LOG ENTRY” button in any popup:

1. Click the instrument on the map.
2. Click ➕ ADD LOG ENTRY.
3. Fill out the Google Form (e.g., problem description, date, action taken).
4. Submit the form.

The entry is stored in the shared log spreadsheet linked as “VIEW HISTORY LOG”.

## How to view instrument history
1. Click the instrument on the map.
2. Click 📜 VIEW HISTORY LOG.
3. Filter or search inside the sheet to see previous incidents, maintenance, or notes.

## How to change coordinates (for map maintainers)
If you move equipment or update the floor plan, you may need to move markers.

1. Go to the live map.
2. Click 📍 Start Aligning Dots (top‑right).
3. Click on the map where the instrument should appear.
4. Copy the coordinates shown in the popup alert.
5. Send these to the map maintainer (or edit the instrumentCoords section in the HTML if you are comfortable with code).

## How to update manual links
Each instrument popup has a VIEW MANUAL button.

If a manual link is wrong or missing:
1. Collect the correct URL (PDF, Google Drive, GitHub, etc.).
2. Tell the map maintainer which instrument and new link to use
(or update the instrumentManuals section in the HTML if you edit the code yourself).

## Who is this for
* Cernak Lab members who want a quick overview of instrument availability.
* New lab members learning instrument locations.
* Anyone coordinating maintenance and scheduling around shared equipment.

## The goal is to keep this tool simple to use: most edits just involve updating the Google Sheet; you only need to touch the code when you move instruments or add new ones.
