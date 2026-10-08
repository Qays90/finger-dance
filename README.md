Finger Dance

Finger Dance is an interactive 3D hand animation project built with Python and Panda3D. Each finger has its own animation targets and timing, producing dance, piano, and wave movements.

The movement logic is inspired by circles and geometric relationships between joints. A spacing guard limits how closely selected joints of neighboring fingers can approach each other.

Download and run on Windows

1. Download finger-dance-windows.zip.
2. Right-click the downloaded ZIP and select Extract All.
3. Open the extracted finger-dance folder.
4. Double-click Start.cmd.

The package includes a 64-bit Windows Python runtime, the required libraries, and the hand model. No separate Python installation or pip commands are needed.

Keep the extracted files together: Start.cmd uses the included runtime, and the application loads the hand model from the project folder.

The project author has tested the Windows package and confirmed that it runs.

Main controls

Control	Action
D	Finger dance
Q	Piano animation
W	Wave animation
A	Automatic animation sequence
F	Fist pose
P	Pointing pose
R	Release pose
B	Raise the index and middle fingers
N	Raise the middle finger
E	Next expressive pose
S / M / H	Low / medium / high bending intensity
Space	Pause or resume finger animation
G	Toggle the joint-spacing guard
C	Toggle visible joint links
Z	Switch camera mode
Left mouse drag	Rotate the camera in free-camera mode
Mouse wheel	Zoom in or out

Close the application window to exit.

Included files

* FingerDance.py — hand animation source.
* run.py — application launcher.
* Start.cmd — Windows startup script.
* R.HandXXX11.glb — hand model.
* hand_aramture.png — hand armature image.
* runtime/ — bundled Python runtime and libraries.
* docs/ — movement explanation and package review notes.

See docs/MOVEMENT.md in the extracted package for the movement calculations.

Movement limits

The spacing guard checks selected joint positions between neighboring fingers. It does not perform full mesh collision detection or physical simulation.

Release

Finger Dance v1.0.0