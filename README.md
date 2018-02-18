# SMHI-NodeRed-HomeAssistant
Directions for getting SMHI data into home-assistant as sensors using Node-Red to parse and output the Json

## Node-Red Flow
Import this into your node-red installation and in the second node named **SMHI JSON** replace the coordinates with your own in the url.
Then in the last node **MQTT Output** make sure that your own mqtt server is selected.

![Node-red Flow](https://i.imgur.com/WEum3H3.png)


## Home-Assistant Sensors and templates
Add these to your sensors in Home-Assistant and reboot, they will then show up as "sensor.smhi_name" in your Home-Assistant install
I also recommend you add the templates to your sensors, that way you will get the wind direction as a text message and not by degrees.

![HASS Sensors](https://i.imgur.com/OqFXdQ2.png)


## Extras
The reason that the sensors and template is split up in this git is that I recommend that you split up your config into directories, that makes maintaining your Home-Assistant configuration much easier and you can just download the .yaml files from this Git and add to your directory

![Folder Structure](https://i.imgur.com/6DkePdT.png)

## Links
* [Information about splitting up your Home-Assisant configuration](https://home-assistant.io/docs/configuration/splitting_configuration/)
* [Svenska Hemautomatiseringsgruppen (Swedish)](https://www.facebook.com/groups/SHgruppen)
* [SMHI Open Data API Docs](http://opendata.smhi.se/apidocs/metfcst/index.html)

## Contributors

Thanks goes to these wonderful people:

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
| <img src="https://avatars1.githubusercontent.com/u/6575206?s=460&v=4" width="100px;"/><br /><sub><b>[Erik Näsström](https://github.com/Naesstrom)</b></sub> | <img src="https://avatars3.githubusercontent.com/u/26795429?s=460&v=4" width="100px;"/><br /><sub><b>[Torbjörn Söderberg](https://github.com/tubalainen)</b></sub> | <img src="https://avatars3.githubusercontent.com/u/2168003?s=460&v=4" width="100px;"/><br /><sub><b>[Johan von Lindström](https://github.com/bhaap)</b></sub>|
| :---: | :---: | :---: |
<!-- ALL-CONTRIBUTORS-LIST:END -->
This project follows the [all-contributors](https://github.com/kentcdodds/all-contributors) specification.
Contributions of any kind are welcome!
