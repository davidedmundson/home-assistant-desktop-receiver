# Home Assistant Desktop Reicever

The goal is to provide a

home-assistant-desktop-reciever is a small autostarting daemon that runs in the user session of a linux desktop.

Currently it only uses the rest APIs of HA, so no changes are needed there.

Whilst most of this would be possible with a lot of manual setup via the command line switches and ssh, this is easier to set up, more extensible and more secure.

It should work on all standard Linux desktops; GNOME, KDE/Plasma, XFCE, whatever that follows the standards

##What it provides

* Notification receiver. HA notifications appear as normal desktop notifications

* A binary "sensor" of whether the computer is not just on, but actually active (not locked and activity within the past n minutes). Useful for automation

* A switch for dpms (screen management)

##Non-goals

I don't intend for this to be a GUI desktop client. There's not a lot of code overlap

##Setup




##Plans

* Replace with MQTT

* Updating HA state directly via web API (means we need to know HA location and auth)

* Make it discoverable on the HA side.
