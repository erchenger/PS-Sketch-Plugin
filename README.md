# PS-Sketch-Plugin
Sketch plugin to export Strings for easy consumption in applications or for localizations. This plugin is in beta so please understand that there is still work to be done. Any issues you have please submit via github issues.

#Installing
- Download the [plugin zip](https://github.com/erchenger/PS-Sketch-Plugin/blob/master/archive/PS-Sketch-Plugin_0.1.0.zip).
- Unzip
- Double click the `ps.sketchplugin` file
- You should be prompted by Sketch to install the plugin

#Sketch Usage
- Change text layer name to include a prefix of `loc_`
 - Exmaple:
   - Text Name: loc_title
    - Text Value: The Title of the string
- Click `plugins>PS>Export Strings`
- After the `strings.json` file is exported a dialog will pop up with it's location

#Consuming with Twine
- Install [Twine](https://github.com/mobiata/twine)
- Create a `twine.txt` file
- Run the following command

```
twine consume-string-file path/to/twine.txt path/to/strings.json --consume-all
```
