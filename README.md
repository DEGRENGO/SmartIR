SmartIR is a component for controlling AC units and TV devices via Infrared controllers. An IR controller such as Broadlink RM is required.

The key features of the component are:
* Support for Base64, Broadlink Hex and Pronto codes.
* Support for external temperature and humidity sensors (Climate platform)
* Support for external on/off sensor that monitors whether your device is actually On or Off. This may be a power monitor sensor.
* Support for voice assistants.

## **Component setup instructions**
Create the folder `custom_components`, if it does not exist, in the home assistant’s config directory. Create the `smartir` folder and copy `__init__.py`, ` climate.py` and `media_player.py` files into it.
Add the following to your configuration.yaml file.

    smartir:
    
## **Platform setup instructions**
<p align="center">
  <a href="Docs/CLIMATE.md"><img src="http://www.tooltip.gr/github_assets/smartir_climate.png" width="400" alt="SmartIR Climate"></a>
</p>

<p align="center">
  <a href="Docs/MEDIA_PLAYER.md"><img src="http://www.tooltip.gr/github_assets/smartir_mediaplayer.png" width="400" alt="SmartIR Media Player"></a>
</p>

## **Update the component**
The component will check for updates each time HA is restarted. When there is a new version, a new Persistent Notification will appear.
Use the services `smartir.check_updates` to manually check for updates and `smartir.update_component` to start the automatic update.

## Links
* [SmartIR Chat on Telegram](https://t.me/smartHomeHub)
* [Discussion about SmartIR Climate (Home Assistant Community)](https://community.home-assistant.io/t/smartir-climate-component/)
