# warp2shng-mqtt_yaml
This yaml configuration file integrates the Tinkerunity Warp 2 Charger (https://www.warp-charger.com/) into SmarthomeNG (https://www.smarthomeng.de/) by using the integrated MQTT module.

Place the 'warp_charger.yaml' file into the 'smarthomeNG/items' directory of your installation and restart smarthomeNG service. Items will be accessible as 'sh.warp_charger.' items.

Note:
Since the Warp Charger out of the box submits a significant amount of data through MQTT (basically anything that is available at the webpage for status and configuration) and not all of this may be significant in a typical SmarthomeNG environment:
- Not all available MQTT messages are represented in the warp-charger.yaml file (at least not yet)
- In case you may want to exclude subscriptions that are already included in the warp-charger.yaml, the simple way of doing this is to delete (or better comment out) those in your yaml file.
