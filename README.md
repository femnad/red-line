red-line
========

Why?
---

When on a laptop, if you do not run a power manager or have no information panel it is easy to lose track of time an lose everything in the running session when battery dies.

Usage
-----

Just run red-line. Backgrounding the process is manual for your inconvenience:

    red-line &

Configuration
-------------

    normal-sleep=60 # Sleep period when battery percentage is above the warning level 
    warning-sleep=5 # Sleep period when battery percentage is below the warning level
    warning-percent=10 # Percentage below which to transition to warning level
    critical-percent=5 # Percentage below which to transition to critical level
    critical-action=shutdown # What to do when battery percentage is below critical (shutdown|suspend|ignore)
    critical-countdown=15 # Number to Countdown from to zero when before performing critical action
    notify=dzen # Notification method (dzen|libnotify)
    dzen-display-time=5 # Time period to show dzen for
    dzen-warning-fg=#808080 # dzen warning foreground color
    dzen-warning-bg=black # dzen warning background color
    dzen-critical-fg=white # dzen critical foreground color
    dzen-critical-bg=#8b0000 # dzen critical background color

