

# What does it do?
Allows Google Assistant to control Kodi, e.g.,

- Play Animal Planet
- Open Spotify
- Open movies 
- Set volume to 50%
- Pause, Stop
- Turn off/on


### The following commandands are fully or partially supported:

- action.devices.commands.appSelect 
- action.devices.commands.setInput
- action.devices.commands.OnOff
- action.devices.commands.mediaClosedCaptioningOff
- action.devices.commands.mediaClosedCaptioningOn (not working)
- action.devices.commands.mediaNext
- action.devices.commands.mediaPause
- action.devices.commands.mediaPrevious
- action.devices.commands.mediaResume
- action.devices.commands.mediaStop
- action.devices.commands.mute
- action.devices.commands.setVolume


### Software needed:
- HomeAutio.Mqtt.GoogleHome - https://github.com/i8beef/HomeAutio.Mqtt.GoogleHome
- MQTT broker
- Node-red - https://www.nodered.org
- Kodi - https://www.kodi.tv

### Setup instructions:
Step 1 
Install the excellent https://github.com/i8beef/HomeAutio.Mqtt.GoogleHome Detailed instruction can be found in the wiki.

Step 2
Install a MQTT broker, e.g., Eclipse Mosquitto.

Step 3
Install Node-red found here https://www.nodered.org
Note: all three above is best installed as docker containers.

Step 4



Step 5







### Todo:
- Document setup
- Complete definition of Kodi
- Complete node-red flows


