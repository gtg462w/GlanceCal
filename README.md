# GlanceCal
Simple iOS Today View extensions/widgets for calendar events scheduled today and tomorrow

<!-- ![Example screenshots](https://raw.githubusercontent.com/jackhallybone/GlanceCal/master/Screenshots.png "Example screenshots") -->

<img src="https://raw.githubusercontent.com/jackhallybone/GlanceCal/master/Screenshots.png"  width='500' alt="Example screenshots">

----

### The Problem

The default iOS Calendar Today View widgets don't make much sense to me. At a glance I only really need to know about events that are scheduled for today and tomorrow.

### The Solution

Make two quick and simple iOS Today View extensions/widgets that presents all the events scheduled for later today and tomorrow.

### Issues

*I don't yet know anything about Swift, iOS development or Xcode*. I like learning by trial and error so this project will probably contain a lot of blinding errors that I don't know about yet (but hopefully none that I do know about...).

----

### To Do:
- Improve implementation of the `formatEventTime` etc methods (annoying to pass `daysFromToday` through several).
- Is notification centre framework required for the extensions, why is it there?
- The order of the events is not so nice (eg., multiday all days are not listed at top...)
- The 'no events' label should go to the calendar app day when pressed
- The 'calendar access required' labels should go to the setting app:GlanceCal when pressed
- Holiday calendar now shows up (didn't before...?) even though it is hidden in calendar app. Should use the shown list in the calendar app if we have access to that information?
- Fix the custom table cell implementation (there must be a cleaner way)
- Handle 12h and 24h display options
- Order the all day events as they are in the calendar app?
- Only need to perform update when there is new data?


### Issues:
- Extensions are limited to the height of the device screen (eg, displays a maximum of 8 events per day on an iPhone SE)


### To Consider:
- Option to choose which calendars are displayed
- Option to hide events when device is locked
- Should I be using a framework to share the `ManageEventData` code?
- Head the extension view with the day of the week and date of the day shown
- Show reminders due today and tomorrow (and any overdue?)
- Show alarms set in the clock app (not possible to access this data)
