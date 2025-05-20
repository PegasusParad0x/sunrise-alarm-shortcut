# Sunrise Alarm (iOS Shortcut)

This is an iOS Shortcut I built that sets alarms before sunrise and gives me a suggested bedtime based on the next morning’s light.

I’m a network engineer. I don’t write code. I just wanted something that helps me keep a consistent routine, and this Shortcut ended up working better than expected.

---

## What it does

- Checks tomorrow's sunrise time using your current location
- Deletes any alarms containing label "Sunrise"
- Creates 3 new alarms:
  - 10 minutes before sunrise
  - 15 minutes before sunrise
  - 20 minutes before sunrise
- Calculates a bedtime (8 hours before sunrise)
- Sends a notification showing that bedtime

---

## How I use it

I set this to run automatically every sunset using the Automation tab in Shortcuts.

It cleans up the old alarms and creates fresh ones, so I always wake up close to sunrise with a few backup alarms. The bedtime reminder is just a nice extra that helps me not stay up too late.

---

## Step Breakdown

1. Find all alarms with the label "Sunrise"
2. Delete them
3. Get sunrise time from the Weather data
4. Subtract 10, 15, and 20 minutes and create alarms for each one
5. Subtract 8 hours from sunrise and send a notification:  
   "Go to bed at [calculated time]"

---

## Ideas for improvement

- Trigger Sleep Focus mode
- Integrate with HomeKit (dim lights or play a sound)
- Add a fallback fixed-time alarm in case weather data fails

---

## Author

Created by PegasusParad0x  
Curious.
