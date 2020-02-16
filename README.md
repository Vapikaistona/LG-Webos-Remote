# LG-Webos-Remote
Similar to the Roku Remote I've shared, I wanted to have a clickable remote control within Home assistant for my new LG WebOStv so here it is if you want it.

![Remote](https://github.com/moistgun/LG-Webos-Remote/blob/master/remote.png)

I am controlling the power toggle on the TV using the built in Media player services in home assistant + the Wake on Lan feature in the docs.

I took the remote image from here, https://dribbble.com/shots/5363712-Universal-TV-Remote-App-Design
And used the picture elements lovelace card to display it and stack buttons over top.

Iddo added support for the magic remote which can alternatively be used if you don't want the generic remote support.

Prerequisites: 

- Home Assistant version 0.104 or greater
- installed LGWebOS component and WOL for powering on: https://www.home-assistant.io/components/webostv/

Steps to setup:

1) Copy the relevant remote image into your /config/www/ folder

2) Copy the relevant lovelace_remote.yaml contents into a manual lovelace card 

3) Replace the Media player entity id with your entity id if its different

*Notes

Sources can be updated to match what you want, but the generic template is setup as such
Red - Netflix
Green - Hulu
Yellow - Plex
Blue - Amazon Prime

I could not get every button to do something that made sense so if you have better luck, please let me know!
In the mean time, the images have placeholder buttons, so you should be able to easily update the remote to your liking.
Currently not operating in the generic image
- Hamburger
- Smart
- 123
- Input
- Record
