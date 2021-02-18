---
layout: page
title: Project Overview
---

![CoverImage](images/CoverImage.png)

# CGM TIR Project Overview

This project began as a collaboration between Dana (T1D,xdrip+,openAPS,NS, Medtronic, Dexcom G6 user) and John (software developer boyfriend).  Dana purchased a Garmin watch to replace her many Pebble watches, but just couldn't find an existing watchface that provided everything she wanted for viewing T1D data.  She sketched out her original idea for a Garmin watchface and John brought it to life using the Garmin SDK.  This page is intended to explain settings, provide insight into our thinking, and share ideas for future development plans in more detail than we can provide in the Connect IQ description.

## Current Projects

- [CGM TIR Garmin Watchface](https://apps.garmin.com/en-US/apps/38c13f6f-3f68-4a08-b58b-1e1089292a6f)

### Watchface Description

CGM TIR watchface provides a clean & simple design that provides users with blood glucose values, trend arrows and deltas, a units remaining in an insulin pump reservoir, openAPS looping status, and a motivational time in range (TIR) ring that can be displayed six different ways.  This watchface can be configured to receive data from xDrip+ (Android only) AND Nightscout to allow glucose data to continue to be displayed without an internet connection OR with data collected from Nightscout only (cell service/internet connection required). Color schemes are fully customizable in the watch configuration settings. The watchface currently displays heart rate, stairs climbed, steps and a step goal progress bar, a phone notification count, watch battery level, bluetooth connectivity, and a watch Do Not Disturb indicator. The pump insulin units remaining are displayed a visual status bar similar to the step goal display.  The watchface is currently optimized for openAPS looping and xDrip+ as the local data source.  If you would like to use Nightscout only without xDrip+, select "Other/None" in the local collector setting.  As of 0.1.0 release, there are now options to display data for two diabetics on the same watchface.  

### Troubleshooting
<details>
 <summary>Data won't load</summary>
  
  ## Check Your Nighscout URL in Settings
  1. Due to memory constraints, 12-24 hours of data must be returned from Nightscout before the watch can begin pulling from a local collector (if set), so if the watch won't load at all, this is the first thing you need to rule out.  
  2. **Your Primary User Nightscout URL** is the only setting that you are **required** to update from the default settings.  
     * Make sure that you have included **https://** at the beginning of the URL, and don't include any additional information beyond **.com**.  
     * If you enter your URL incorrectly, you may have to wait up to 5 additional minutes after fixing this setting for data to populate - please be patient!
  3. If you just switched from a Garmin activity or a watch app back to the watchface, you need to wait for the data to reload.  This can take up to 10 minutes for a single user and up to 15 minutes if using the watch to follow two diabetics.  
  4. If you have entered 2 nightscout URLs to follow two diabetics using this watchface, it can take up to 15 minutes before data is current.  Due to extremely limited memory constraints of many Garmin watches, it is necessary to wait 5 minutes after pulling the 24-hour TIR data for the first user before it can be pulled for the 2nd user.  Then another 5 minutes must pass before the most recent SGV values can be pulled.

</details>
<details>
 <summary>TIR ring segments are incorrect</summary>
  
  ## Check Range & Ring Settings
  1. Make sure that your Target Range High and Low values are in the correct units.  If you picked mg/dL, make sure your range values are expressed that way.  If you chose mmol/L, make sure your range values are expressed that way (the default settings will not make sense in mmol/L).  
  2. If there is a gap in your data that you weren't expecting, you may have selected Noon/Midnight reset instead of Rolling/Continuous reset. Noon/Midnight reset will only show you data from 12a or 12p (whichever was more recent) to the current time, so you will see a gap in the data from the current time clockwise back to 12a or 12p.   
</details>
<details>
 <summary>Icons/values disappeared</summary>
 
 ## Check Color Choices & Stale Data
  1. If your background color is the same as any of your other color choices, those items will not be visable on the watchface.  If you choose a background color that is similar to your icon/foreground color, items may be present but difficult to see.   
  2. If your data source has reached the Stale Data Urgent threshold that you set, icons and values from that data source will disappear from the watchface.  
   * Check to make sure your watch is in range of your phone. 
   * If nightscout data is lost, check to see if you have cell/internet connection
</details>


### Have the developers considered...?

### What's up next in development?
- CGM TIR Watchface supporting two T1Ds
- Adding additional local collector options

### Support or Contact

Use the _Contact Developer_ option for the watchface in the [Garmin Connect IQ Store](https://apps.garmin.com/en-US/apps/38c13f6f-3f68-4a08-b58b-1e1089292a6f)

