# OBS Applause

During Corona, many musicians were deprived of their stages. 
Looking for solutions to share their art with their fans despite the circumstances,
livestreaming via Twitch was almost perfect.
However, these artists are missing a very basic element: The reactions of their audience.

This project aims to fix that, well... to some extent.

The idea is as follows: The tool pays attention to what's going on in the chat and displays small overlays in the video stream accordingly.
For example, if a 👏 appears in the chat, a clapping animation is played. The more people "applaud", the more crowded the image becomes.

## Architecture

The Repo contains multiple Packages:

* obs-applause-admin: Contains the Administration interface for the tool.
* obs-applause-render: Contains the "renderer" which can be included in OBS
* obs-applause-server: Contains the code for the Server, listening to the chat and triggering the animations.

The communication between the websites and the server uses Apollos graphql.
