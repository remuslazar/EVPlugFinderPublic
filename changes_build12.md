## [V0.1 Build 12](https://github.com/remuslazar/EVPlugFinderPublic/milestone/5?closed=1)

See also https://github.com/remuslazar/EVPlugFinderPublic/milestone/5?closed=1

Release Date: 2016-12-21

- bugfix in "Fault Report" handling. Faulty stations now being detected as such
- Cosmetic changes in the ChargePoint Detail View, labels, ordering,..
- App reload current location and charging stations neadby if started after > 2 minutes after suspended timestamp (this timeout can be tweaked in future releases)
- Reload and List Button logic (enable/disable) streamlined with the App logic
- Network Request Timeout 15 seconds (default was 1 minute)
- Performance in very bad network situations improved
- Reload button turns red if a network error occurred
