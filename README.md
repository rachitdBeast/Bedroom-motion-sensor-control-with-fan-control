# Bedroom-motion-sensor-control-with-fan-control

## Features

    *- Several motion sensors; "no motion" actions only run when ALL sensors are off.
    *- Lights: time window, sun elevation rule, brightness, optional ambient scene.
    *- Manual override (on/off option, no helpers needed): the last activity of each light/fan is
      checked. If it was last turned OFF by a logged-in user (Home Assistant app or dashboard,
      or a voice assistant that passes the user), motion will not turn it on again until you
      turn it back on yourself. Changes with no user attached (automations, power loss and
      restore, a physical switch cutting power) are never treated as a manual override.
    *- Sleep mode: a toggle (input_boolean or switch). While it is ON the motion automation is
      blocked, for example for an afternoon nap.
    *- Ceiling fan: delayed start (so a quick walk-through does not start it), soft start at a lower
      speed, extra run-on time after lights go off, and an optional minimum temperature.

### Based on https://github.com/arturoliveira/home-assistant/blob/main/advanced_custom_motion_sensor.yaml
### Requires Home Assistant 2024.10 or newer.
