# Submitting on moodle 
To submit a project on moodle it requires the following

## APP files
Open up your Unity project folder. You will need to add (compress) the following folders to a .zip file.
* Assets
* Packages
* Project Settings

Submit the .zip file

## Game Build

### Itch.io build
#### Setup
1. Create and account on Itch.io
2. Follow steps on Itch.io to create a new project
3. Ensure you upload the build that you create below
4. Ensure that the game is viewable by me, but not public to all of itch.io  (Instructions coming later)

#### WebGL Build
(You will have to have installed WebGL in unityhub (Instructions coming later))

1. Go to “File”, click on “Build Settings”
1. In the Build Settings window, select “WebGL” as the target platform
1. Click on “Switch Platform” to set WebGL as the active platform
1. Click on “Player Settings” to open the Player Settings window
1. In the Player Settings window, you can configure various settings such as the name of the game, the default screen resolution, and the logo that will be displayed on the loading screen
1. Click on “Add Open Scenes” to add the current scene to the build
1. Click on “Build” and choose a directory to save the build

You might need to remove compression for your game

1. Go to Unity > File > Build Settings > Player Settings > Compression.
  * Option 1) There, disable Compression, and enable Decompression Fallback.
  * Option 2) If the previous doesn’t work, select GZIP compression and enable Decompression Fallback.



### Windows build
With your project open in unity.
1. Go to File, Build Settings...
2. Ensure that your scenes are in the "Scenes In Build" section near the top of the screen. (You can drag your scenes in or click "Add Open Scenes").
3. Make sure "Target Platform" says "Windows"
4. Click "Build" or "Build And Run", the latter allows you to run the game instantly for testing.
5. Choose the folder your build will be saved in. Normally saved in a folder called "Build" in your project.
6. Add your whole build folder to a .zip file.
7. Submit the .zip file

## Git Link
Create a git repo for your project, [click here to learn how](https://github.com/CapelaGames/csProgrammingBasics/blob/main/git.md)

If you open your git repo on github, you can copy and paste the URL into the submission text field. Don't forget to make your project public so it can be used for marking.

## Documentation
Please submit your project's documentation as a .pdf
1. Open your documentation in word (or other editor).
2. Click File, Save As
3. Choose PDF
4. Submit the PDF (NOT in a .zip)
