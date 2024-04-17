CCK-PlayTogether
===================

**CCK-PlayTogether** is an Unity project template for creating CCK Props that interact with CVR-PlayTogether in ChilloutVR.

Requirements
===================

- Windows 10 or above
- Unity 2021.3.23f1
- ChilloutVR CCK v3.7
- Latest uWindowsCapture modified for CVR-PlayTogether (https://github.com/Searaphim/uWindowCapture/releases)
- Latest PlayTogetherLib DLL (https://github.com/Searaphim/CCK-PlayTogether/releases)

How to use
----------

- Launch the project in Unity (or make a new one based on this template)
- Import ChilloutVR's CCK
- Import the modified uWindowCapture AND uncheck Plugins/x86 (You will get errors about missing types or namespaces. This is normal.)
- Copy/Paste the PlayTogetherLib DLL at the root of 'CCK-PlayTogether/Assets/uWindowCapture'
- Load the 'PropScene' Scene found in 'CCK-PlayTogether/Assets/Scenes'
- If you're getting a missing script on the 'Desktop' prop prefab; you must open the prefab and set the script to point to 'uwcWindowTexture'
- close and reopen the project and make sure you don't have any errors left.
- On the 'Desktop' prop: edit these parameters of the 'uWc Window Texture' Component:
	- Type = Desktop
	- Capture Frame Rate = 30
- Test that it works by hitting the Play button. The Scene should be displaying your current Desktop #0
- You are now ready for upload. Use this as an example for your custom props.