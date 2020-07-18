# What does it do?

![nest-hub.jpg](https://raw.githubusercontent.com/sognen/homeautio-config/master/kodi/images/nest-hub.jpg)

Allows Google Assistant to control Kodi, e.g.,

* Switch to a tv channel
* Return to the last/previous channel the user was on.
* Adjust the current channel by a relative amount.
* Playback commands such as pause, stop, next and previous
* Open addons on Kodi, e.g., Youtube, Spotify and movie library.
* Set volume and mute

### Software needed:

* HomeAutio.Mqtt.GoogleHome - https://github.com/i8beef/HomeAutio.Mqtt.GoogleHome
* MQTT broker
* Node-red - https://www.nodered.org
* Kodi - https://www.kodi.tv

### Setup instructions:

Step 1

* Install the excellent https://github.com/i8beef/HomeAutio.Mqtt.GoogleHome Detailed instruction can be found in the wiki.
* Install a MQTT broker, e.g., Eclipse Mosquitto.
* Install Node-red found here https://www.nodered.org Note: all three above is best installed as docker containers.

Step 2

* Copy googleDevices.json into folder HomeAutio config folder

Step 3
* Import nodered.json into your nodred
* The following nodes need to be installed and configured: node-red-contrib-kodi, node-red-contrib-mqtt-broker

Step 4

Step 5 Say "sync my devices" to your Google Assistant device.

### Todo:

* Document setup
* Complete definition of Kodi
* Complete node-red flows