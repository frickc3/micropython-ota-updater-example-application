# micropython-ota-updater-example-application

This is an example application for the OTA Updater with more detailed information found at [github.com/bensherlock/micropython-ota-updater](https://github.com/bensherlock/micropython-ota-updater).

## Usage

Copy the contents of main/ to the root directory of the PYBD USB MSD.

Create a wifi_cfg.json file using the template as an example and populate with appropriate SSID and PASSWORD values. Note that .gitignore is set to ignore this config file in this repository. 

On POR (Power On Reset) the program will attempt to connect to the wifi and then check GitHub for the latest release versions of the modules (ota_updater and example_module) and then download them before rebooting the device. After running you should now see these modules updated.
