
# Dynamic Watch Faces with Tag Expressions
Creating compelling watch faces goes beyond static designs. Tag expressions in Watch Face Studio empower designers like you to achieve this dynamism without writing a single line of code.

## What are Tag Expressions?

Think of tag expressions as mini-programs running within watch face. They use real-time data from the watch—like time, date, battery level, and sensor data—to control how elements on watch face behave. These expressions are built using tags, which are keywords enclosed in square brackets [] that represent specific data points.

## Key Components
- __Tags__: These are the data sources. Some common tags include:
  
  - `[HOUR]`: Current hour (0-23 or 1-12 depending on settings).
  - `[MINUTES]`: Current minutes (0-59).
  - `[SECONDS]`: Current seconds (0-59).
  - `[BATT_PER]`: Battery percentage (0-100).
  - `[IS_CHARGING]`: Charging status (1 for charging, 0 for not charging).
  - `[DATE_DAY]`: Day of the month.
  - `[DATE_MONTH]`: Month of the year.

- __Operators__: You can combine tags with mathematical operators (+, -, *, /, %), comparison operators (>, <, =, !=), and logical operators (&&, ||, !) to create conditions.

- __Conditional Expressions__: The ternary operator ? : allows for conditional logic. The syntax is `[condition] ? [value_if_true] : [value_if_false].`

## Practical Examples: Task 1
- __Step 1__: Install the __Watch Face Studio__.
- __Step 2__: Design the watch face on free hand.
  - Add background
  - Set watch to __Analog__ mode
  - Add the hands(hour, minute, second)
  - Add Progressbar on left bottom corner
  - Add text box center of the circular progressbar
- __Step 3__: Set condition on color of progress bar 
  - `[BATT_PER] <= 20 ? #FF0000 :rgb(18, 131, 121)`

## Conclusion
Tag expressions unlock a new level of customization and interactivity for watch face designers. By leveraging these powerful tools, you can create dynamic, informative, and truly unique watch faces that enhance the user experience. Start experimenting, and let your creativity flow!