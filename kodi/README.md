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
* Node-red - https://www.nodered.org (optional)
* Kodi - https://www.kodi.tv or any other mediaplayer that can be controlled with MQTT.


### Hardware needed:
* A device that can run Kodi
* A device that can run HomeAutio, MQTT broker and Node-red. You may run these and Kodi on the same device.
* Audio/video amplifier (optional) - Note: see instructions below on how to control input switching and volume.

### Setup instructions:

#### Step 1
* Install the excellent https://github.com/i8beef/HomeAutio.Mqtt.GoogleHome Detailed instruction can be found in the wiki.
* Install a MQTT broker, e.g., Eclipse Mosquitto.
* Install Node-red found here https://www.nodered.org Note: all three above is best installed as docker containers.

#### Step 2
* Copy googleDevices.json into folder HomeAutio config folder
Note: the googleDevices.json file containts all my devices You may only be interessted in /ivingroom/kodi. 

#### Step 3
This step can be skipped if you already have a bridge between Kodi and your MQTT broker.
* Import nodered.json into your node-red
* Install the following nodes: 
  - node-red-contrib-kodi 
  - node-red-contrib-mqtt-broker
  - node-red-contrib-openhab2 (optional)

#### Step 4
Coplete A or B depending on your setup.

##### A - Amplifier controlled input switching and volume control.
To be written.

##### B - Kodi volume control
To be written.

#### Step 5 
Say "sync my devices" to your Google Assistant device. 

You should now be able to control your Kodi using your voice.

## Todo:
* Document setup
* Complete definition of Kodi
* Complete node-red flows
