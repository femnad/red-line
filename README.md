red-line
========

Why?
---

When on a laptop, if you do not run a power manager or have no information panel it is easy to lose track of time and lose everything in the running session when the battery dies.

How?
----

Just run red-line. Backgrounding the process is manual for your inconvenience:

    red-line &

Sends messages via `notify-send` so a running notification daemon is necessary.

Configuration
-------------

Default configuration values:

    normal-sleep=60 # Sleep period when battery percentage is above the warning level
    warning-sleep=5 # Sleep period when battery percentage is below the warning level
    warning-percent=10 # Percentage below which to transition to warning state
    critical-percent=5 # Percentage below which to transition to critical state
    critical-action=shutdown # What to do when battery percentage is below critical (shutdown|suspend|ignore)
    critical-countdown=10 # Number to countdown from to zero before performing the critical action

Expecting the configuration file to be on `$HOME/.redline`
