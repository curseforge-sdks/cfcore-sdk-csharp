# cfcore-unity-ui

This readme file contains information on how to get started with adding the cfcore UI component into your game.

## Setup your game

To get started, follow these steps:

- Unzip the cfcore-unity-ui-x.y.z.zip into your project's Assets folder (usually it will reside in a top-level folder named: cfcore-unity-ui)
- Drag the ApiManager prefab to your scene
- Drag the CFCoreModBrowser prefab to your scene (Import TMP Essentials if required)
- Some versions of Unity will require you to add the UnityEngine.InputSystem package (Window > Package Manager - select Unity Registry and install Input System) - restart Unity editor after this step
- An "Eternal" menu item should now appear (next to Window) - Select it and then "Edit Settings" to fill in the Game Id and the Api Key of your game:
  - If you haven't already, create an account on https://console.curseforge.com/ + add a game to your account
  - Use the Game Id and the Api key of your game to fill in the ApiManager prefab in the READ_APIManager script the coresponding fields

For more information please read https://docs.curseforge.com/#getting-started

## Sample Scene

The sample scene is a demo that includes everything you need to browse and
download the mods for a game.

## Usage

The Api is ready to use.

- You may create your own UI and access it through READ_APIManager e.g use
READ_APIManager.Instance.SearchMods in order to find mods in accordance to the
pagination and search parameters

For more information please read https://docs.curseforge.com/#accessing-the-service

- This package includes prefabs that implement the most common functionality
that you will in your game. You are free to use them at your discretion.
  - CFCoreModsBrowser : A multi purpuse Prefab that allow the following functions:
    - Browse mods
    - Download mods
    - Uninstall mods
    - Like/Unlike mods
  - Popup-UploadMod : A Popup that allow the user to upload new mods and update
 existing ones. This package includes SampleCFCoreUploadMod which is an example of usage of this popup and a few use cases.You can find it in the
 "SampleUploadMods" folder.

For more information please read the README file in the "Readme" folder.

## More info

You can find another README files in :
.../Assets/cfcore/cfcore-unity-ui/readme-files/UploadModReadMe.md : A more thorough explanation about how to upload mods

For more info about the API please visit https://core.curseforge.com/
For more developer actions and moderation please visit https://console.curseforge.com/#/
You can also create and browse mods from our main site https://www.curseforge.com/YOURGAMENAME/

Join our Discord server
