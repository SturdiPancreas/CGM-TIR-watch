---
layout: default
title: Home
---

![CoverImage](images/CoverImage.png)

This project began as a collaboration between Dana (T1D,xdrip+,openAPS,NS, Medtronic, Dexcom G6 user) and John (software developer boyfriend).  Dana purchased a Garmin watch to replace her many Pebble watches, but just couldn't find an existing watchface that provided everything she wanted for viewing T1D data.  She sketched out her original idea for a Garmin watchface and John brought it to life using the Garmin SDK.  This page is intended to explain settings, provide insight into our thinking, and share ideas for future development plans in more detail than we can provide in the Connect IQ description.

## Current Projects

- [CGM TIR Garmin Watchface](https://apps.garmin.com/en-US/apps/38c13f6f-3f68-4a08-b58b-1e1089292a6f)

### Watchface Description

CGM TIR watchface provides a clean & simple design that provides users with blood glucose values, trend arrows and deltas, a units remaining in an insulin pump reservoir, openAPS looping status, and a motivational time in range (TIR) ring that can be displayed six different ways.  This watchface can be configured to receive data from xDrip+ (Android only) AND Nightscout to allow glucose data to continue to be displayed without an internet connection OR with data collected from Nightscout only (cell service/internet connection required). Color schemes are fully customizable in the watch configuration settings. The watchface currently displays heart rate, stairs climbed, steps and a step goal progress bar, a phone notification count, watch battery level, bluetooth connectivity, and a watch Do Not Disturb indicator. The pump insulin units remaining are displayed a visual status bar similar to the step goal display.  The watchface is currently optimized for openAPS looping and xDrip+ as the local data source.  If you would like to use Nightscout only without xDrip+, select "Other/None" in the local collector setting.  As of 0.1.0 release, there are now options to display data for two diabetics on the same watchface.  



### Have the developers considered...?

### What's up next in development?
- CGM TIR Watchface supporting two T1Ds
- Adding additional local collector options

### Support or Contact

Use the _Contact Developer_ option for the watchface in the [Garmin Connect IQ Store](https://apps.garmin.com/en-US/apps/38c13f6f-3f68-4a08-b58b-1e1089292a6f)

