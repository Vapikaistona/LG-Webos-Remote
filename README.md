# LG-Webos-Remote
Similar to the Roku Remote I've shared, I wanted to have a clickable remote control within Home assistant for my new LG WebOStv so I took advantage of a few things to stitch one together.

![Remote](https://github.com/moistgun/LG-Webos-Remote/blob/master/remote.png)

I am controlling the power toggle on the TV using the built in Media player services in home assistant + the Wake on Lan feature in the docs.

I took the remote image from here, https://dribbble.com/shots/5363712-Universal-TV-Remote-App-Design
And used the picture elements lovelace card to display it and stack buttons over top.

Prerequisites: 

- Home Assistant version 0.104 or greater
- installed LGWebOS component and WOL for powering on: https://www.home-assistant.io/components/webostv/

Steps to setup:

1) Copy the remote.png image into your /config/www/ folder

2) Copy the lovelace_remote.yaml contents into a manual card

3) Replace the Media player entity id with your entity id if its different

*Notes

Sources can be updated to match what you want, but this template is setup as such
Red - Netflix
Green - Hulu
Yellow - Plex
Blue - Amazon Prime

I could not get every button to do something that made sense so if you have better luck, please let me know!

Currently not operating in the image
- Hamburger
- Smart
- 123
- Input
- Record
