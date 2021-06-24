---
layout: default
title: Home
---

![CoverImage](images/CoverImage.png)

This project began as a collaboration between Dana (T1D, xDrip+, OpenAPS, Nightscout, Medtronic, Dexcom G6 user) and John (software developer boyfriend).  Dana purchased a Garmin watch to replace her many Pebble watches, but just couldn't find an existing watch face that provided everything she wanted for viewing T1D data.  She sketched out her original idea for a Garmin watch face and John brought it to life using the Garmin SDK.  This page is intended to explain settings, provide insight into our thinking, and share ideas for future development plans in more detail than we can provide in the Connect IQ description.

## Current Projects

- [CGM TIR Garmin Watchface](https://apps.garmin.com/en-US/apps/38c13f6f-3f68-4a08-b58b-1e1089292a6f)

### Watch Face Description

CGM TIR watch face provides a clean & simple design that provides users with blood glucose values, trend arrows and deltas, a units remaining in an insulin pump reservoir, OpenAPS looping status, and a motivational time in range (TIR) ring that can be displayed six different ways.  This watch face can be configured to receive data from xDrip+ (Android only) AND Nightscout to allow glucose data to continue to be displayed without an internet connection OR with data collected from Nightscout only (cell service/internet connection required). Color schemes are fully customizable in the watch configuration settings. The watch face currently displays heart rate, stairs climbed, steps and a step goal progress bar, a phone notification count, watch battery level, bluetooth connectivity, and a watch Do Not Disturb indicator. The pump insulin units remaining are displayed a visual status bar similar to the step goal display.  The watch face is currently optimized for OpenAPS looping and xDrip+ as the local data source.  If you would like to use Nightscout only without xDrip+, select "Other/None" in the local collector setting.  As of 0.1.0 release, there are now options to display data for two diabetics on the same watch face.  



### Have the developers considered...?
-  <strong>Adding alerts/vibrations</strong>
Due to Garmin SDK limitations, alerts/vibrations cannot be added to a watch face.  There is the possibility of adding these in the future as a Garmin watch app,    which allows for additional funtionality.

-  <strong>Making the watch compatible with older models like the Forerunner 235 or with Garmin "bike computer" models</strong>
Older Garmin devices can only support the data request needed to display CGM data through an app, not a watch face.  We hope to develop a Garmin watch app in the future that may expand compatibility to older devices.  You can see a list of compatible devices for our current project by visiting the [Garmin Connect IQ Store](https://apps.garmin.com/en-US/apps/38c13f6f-3f68-4a08-b58b-1e1089292a6f) and clicking on the compatible devices tab.  While we have tested the listed devices in the simulator that Garmin provides in their SDK, we have found that the simulator does not always match actual watch function.

### What's up next in development?
- Devices with AMOLED screens need larger fonts and icons.

- The date and time will be made larger.

- The spacing of items on the screen will be adjusted so that there is no overlap.

### Support or Contact

Use the _Contact Developer_ option for the watch face in the [Garmin Connect IQ Store](https://apps.garmin.com/en-US/apps/38c13f6f-3f68-4a08-b58b-1e1089292a6f)

Like what we're doing with this project? [Buy us a coffee](https://www.buymeacoffee.com/cgmtir) to acknowledge the time and work that goes into support and future development. 

