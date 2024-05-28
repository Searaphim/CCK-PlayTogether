CCK-PlayTogether
===================

**CCK-PlayTogether** is an Unity project template for creating CCK Props that interact with [CVR-PlayTogether](https://github.com/Searaphim/CVR-PlayTogether) in ChilloutVR.

Requirements
===================

- Windows 10 or above
- Unity 2021.3.23f1
- ChilloutVR CCK v3.7

HOW-TO
----------

- Simply import the CCK-PlayTogether.unitypackage from the github's Release page into your project.
- There is a pre-made Scene and well as a Prop Screen prefab inside.
- Upload.

Setting up your own CCK-PlayTogether Prop
----------

- Get the repo's latest release (the zipped source code or clone via git)
- Launch the project in Unity (or make a new one based on this template)
- Import ChilloutVR's CCK
- From here you can build your own uWindowCapture if you really want to (otherwise ignore this step). See the [instructions](https://github.com/Searaphim/uWindowCapture)
- Import the latest custom uWindowCapture package or your own AND uncheck `'Plugins/x86'` if present (You will get errors about missing types or namespaces. This is normal.)
- Copy/Paste the latest [PlayTogetherLib DLL](https://github.com/Searaphim/CCK-PlayTogether/releases) (if you built CVR-PlayTogether yourself use `'CVR-PlayTogether/PlayTogetherLib/bin/Debug/netstandard2.1/CVRPlayTogetherLib.dll'` *Not the ILMerge'd one!*) to the root of `'CCK-PlayTogether/Assets/uWindowCapture'`
- Load the 'PropScene' Scene found in `'CCK-PlayTogether/Assets/Scenes'`
- If you're getting a missing script on the 'PropScreen' prop prefab; you must open the prefab and set the script to point to 'uwcWindowTexture'
- close and reopen the project and make sure you don't have any errors left.
- On the 'PropScreen' prop: edit these parameters of the 'uWc Window Texture' Component:
	- Type = Desktop
	- Capture Frame Rate = 30
- You are now ready for upload. Use this as an example for your custom props.
