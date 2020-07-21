# What does it do?

![nest-hub.jpg](https://raw.githubusercontent.com/sognen/homeautio-config/master/kodi/images/nest-hub.jpg)

Allows Google Assistant to control Kodi, e.g.,

* Switch to a specific tv channel
* Playback commands such as pause, stop, next and previous
* Open addons on Kodi, e.g., Youtube, Spotify and movie library.
* Set volume and mute
* Direct play of movie title
* Display movies by title or actor on the TV


### Software needed:
* HomeAutio.Mqtt.GoogleHome - https://github.com/i8beef/HomeAutio.Mqtt.GoogleHome
* MQTT broker
* Node-red - https://www.nodered.org (optional)
* Kodi - https://www.kodi.tv or any other mediaplayer that can be controlled with MQTT.


### Hardware needed:
* A device that can run Kodi
* A device that can run HomeAutio, MQTT broker and Node-red. You may run these and Kodi on the same device.
* Audio/video amplifier (optional) - Note: see instructions below on how to control input switching and volume.

### Setup instructions -  Google Smart Home platform:

#### Step 1
* Install the excellent https://github.com/i8beef/HomeAutio.Mqtt.GoogleHome Detailed instruction can be found in the wiki.
* Install a MQTT broker, e.g., Eclipse Mosquitto.
* Install Node-red found here https://www.nodered.org 
Note: all three above is best installed as docker containers. You can find a sample docker-compose file in this repository.

#### Step 2
* Copy googleDevices.json into folder HomeAutio config folder
Note: the googleDevices.json file containts all my devices You may only be interessted in /livingroom/kodi. 

#### Step 3
This step can be skipped if you already have a bridge between Kodi and your MQTT broker.
* Import nodered.json into your node-red
* Install the following nodes: 
  - node-red-contrib-kodi 
  - node-red-contrib-mqtt-broker


#### Step 4
Coplete A or B depending on your setup.

##### A - Amplifier controlled input switching and volume control.
To be written.

##### B - Kodi volume control
To be written.

#### Step 5 - Setup TV channels
Channel switching by voice is supported if Trait action.devices.traits.Channel is updated with the tv channels available to you.

{
  "availableChannels": [
    {
      "key": "1438667575",
      "names": [
        "animal planet"
      ],
      "number": "103"
	}
}	  
If you have a lage number of  channels you may want to import and run the channel-list.json file to have the channels generated from you automatically.


#### Step 6 - We are done!
Say "sync my devices" to your Google Assistant device. 

You should now be able to control your Kodi using your voice. 


### Setup instructions -  Kodi chatbot
The Kodi chatbots that are capable of natural and rich interactions with users, e.g.,
* Play a specific movie title
* Display recomended, popular, trending and latest movies on the TV
* Search for movies by title
* Search for movies by actor

#### Step 1
<write: install and configure node>

#### Step 2
<write: import agent>

#### Step 3
<write: import flow>

#### Step 4
<write: cigar>


# Voice commands
<write: list voice commands and result>



