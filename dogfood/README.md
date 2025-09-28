# ESPHome Dog Feeding Tracker

This ESPHome configuration works with a M5Stack Core2 v1.1 to track when the dog food container is opened, and reports it to Home Assistant. Additionally, the display on the M5Stack Core2 will display a counter and date of last feeding.

There are two versions:

- `dogfood-accelerometer.yaml` uses the M5Stack Core2's built in accelerometer to determine that the feeder has been opened. Mount your M5Stack unit on the lid of the dog food container.
- `dogfood-sensor.yaml` uses a digital sensor connected to GPIO32 on PortA (the "Grove" connector) to determine when the food has been opened. You can use a hall effect sensor and a magnet on the lid, a reed switch, or even a photocell inside the food container and use that to trigger the feeding event.
