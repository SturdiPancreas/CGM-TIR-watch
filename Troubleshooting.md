---
layout: page
title: Troubleshooting
---

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
