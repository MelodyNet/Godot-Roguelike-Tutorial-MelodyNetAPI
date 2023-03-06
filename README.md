# Godot-Roguelike-Tutorial-MelodyNetAPI
This is a fork of [MateuSai's Godot-Roguelike-Tutorial](https://github.com/MateuSai/Godot-Roguelike-Tutorial) to demonstrate how to use MelodyNet API to add music to your games


## Requirements
You will need:
- Spotify Premium account
- Godot Engine (can be downloaded for free from the [Godot Engine website](https://godotengine.org/))

## Instructions

1. Go to the [MelodyNet Website](https://melodynet-web.vercel.app) to register your account

2. After you're logged in, connect your Spotify (Premium account required) by clicking this button in your dashboard. You will then be redirected to a Spotify login page where you need to log in using your Spotify credentials.

&emsp; <img width="949" alt="image" src="https://user-images.githubusercontent.com/42020364/221728485-094aacbf-d755-49d3-827f-ec2d973754cb.png">

- Currently, our app is in development mode so you will also need to contact us directly to authorize your Spotify account with our API in addition to this step

3. Create your API key by clicking "API Key" in your dashboard and "Generate New API Key". Copy it somewhere as it will be used later on.

4. Clone this repository.

5. Open Godot Engine, click "Import" and open the project.godot file in your repository directory.

<img width="1025" alt="image" src="https://user-images.githubusercontent.com/42020364/221731790-67672f61-ecfa-49fb-894c-3067683ded4e.png">

5. Open the game and paste your API key from step 3 in Rooms.gd where it says `var api_key = "enter your API key here"`

<img width="1385" alt="image" src="https://user-images.githubusercontent.com/42020364/221733007-8b8af5e9-a534-4e0e-859c-b226ad69ff94.png">

6. Open Spotify (desktop/mobile app or web player) and start playing any random song.

7. Click the play button in the top right corner of the Godot Engine window to start playing the game.

- The API will be called every time a new floor starts, playing a new song on your Spotify. Normal floors will play a happy song, while boss floors will play motivational songs.

8. (Optional) For a more seamless transition between songs, you can turn on the "Crossfade songs" option in your Spotify settings.
<img width="865" alt="image" src="https://user-images.githubusercontent.com/42020364/221731826-83f9ca7a-718b-497c-a885-3752202be191.png">

## Troubleshooting
- The output window in Godot Engine will let you see what mood is being requested and what the response code and track ID are.
- If you are getting a response code of 500, check to see if you are currently playing a song as specified in step 6.
