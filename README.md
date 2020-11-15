# Node-PAD

Node-PAD is Node-RED for iPad.

![Alt text](preview.png?raw=true "Preview")

A programming tool for wiring together hardware devices, APIs and online services in new and interesting ways.


It provides a browser-based editor that makes it easy to wire together flows using the wide range of nodes in the palette that can be deployed to its runtime in a single-tap.

Notice: This is not compatible with many nodes in the official repository due to ios security restrictions and device limitations.


Pre-installed nodes:

dashboard, ui-table ui-list ui-vega ui-lineargauge ui-value-trail ui-heatmap ui-media ui-led ui-level ui-state-trail ui-statechart ui-svg ui-contextmenu ui-week-schedule dashboard-bar-chart-data, alexa, email

## References:

Node-PAD: [https://apps.apple.com/us/app/node-pad/id1534470128](https://apps.apple.com/us/app/node-pad/id1534470128)<br/>
Node-RED: [https://nodered.org/](https://nodered.org/)

## About this fork

This branch will be the official copy of what will be published on the app store. It is expected that there will be a lag from every official release of the original project.

## Requests & Getting Help

Feel free to post any issues that you may find in the app to this repo.

If any requests and suggestions just contact me at meku@uchu-neko.com and add node-pad in your subject.

## What's new with Node-PAD v1.1?

 ✔ merge v1.1.3 -> v1.2.1 @done (20-10-20 00:50) <br/>
 ✔ the prebuilt admin authentication can be enabled creating a adminAuth.json file @done (20-11-02 14:19) <br/>
 ✔ admin dark theme that syncs with your ios settings @done (20-10-20 00:50) <br/>
 ✔ itunes file sharing for workflows and installed nodes @done (20-10-20 00:50) <br/>
 ✔ nodes for device data like ip address, battery, cpu, ram, disk, geolocation, accelerometer, etc. @done (20-11-02 14:19)<br/>
 ✔ sqlite.js node running on purely on javascript with web assembly @done (20-11-02 14:22)<br/>
 ✔ You can use static assets now by createing the node-static folder @done (20-11-02 14:23)<br/>

## Low Priority / Future Todos

 ☐ write a 'peertalk node' to enable the use of high speed tcp messaging on the USB port of the ios device<br/>
 ☐ enable the use of Bluetooth or BLE, (apple has a very restrict policy on the usage of this one)<br/>
 ☐ enable the use of non-mfi ESC/POS thermal printer using the bluetooth<br/>

## Important Notes

### ALL YOUR EXISTING FLOWS WILL BE REMOVED

Please backup all your flows before updating to 1.2.1.
If you already made the upgrade, check https://github.com/michaelmruta/node-pad on how receover your old flows.

- If you already upgraded from v1.1.3 to v1.2.1, your old flows will be moved inside a different folder '/var/mobile/Data/Application/.../Documents'.
You should move the contents of this file 'Documents' without file extension to your new flows file found in your document's root folder, eg. flows_My-iPad.json. You can use Finder if your on OSX catalina or the apple Files app in your ios device.

- Another way is to copy the files in your Desktop, perform these commands in your terminal and put it back to your device after.
```
cd ~/Desktop
find var -name "Documents" -exec cat {} \; > flows_*.json
```

## Copyright

Node-RED is a trademark of OpenJS Foundation and other contributors, https://openjsf.org under [the Apache 2.0 license](LICENSE).

Node-PAD is a port of Node-RED for iPhone/iPad and the author of this port is not affiliated with or endorsed by them.
