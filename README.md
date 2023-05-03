# Avatarify-repo
![image](https://user-images.githubusercontent.com/75305634/235898182-a83ac1fd-ce58-4a7b-ad43-57cb6c18e016.png)
https://github.com/alievk/avatarify-python/blob/master/docs/README.md#requirements

Requirements
You can run Avatarify in two modes: locally and remotely.

To run Avatarify locally you need a CUDA-enabled (NVIDIA) video card. Otherwise it will fallback to the central processor and run very slowly. These are performance metrics for some hardware:

GeForce GTX 1080 Ti: 33 frames per second
GeForce GTX 1070: 15 frames per second
GeForce GTX 950: 9 frames per second
You can also run Avatarify remotely on Google Colab (easy) or on a dedicated server with a GPU (harder). There are no special PC requirements for this mode, only a stable internet connection.

Of course, you also need a webcam!

WINDOWS
https://youtu.be/lym9ANVb120

Install [Miniconda Python 3.8](https://docs.conda.io/en/latest/miniconda.html#windows-installers).
Install[ Git](https://git-scm.com/download/win).
Press Windows button and type "miniconda". Run suggested Anaconda Prompt.
Download and install Avatarify (please copy-paste these commands and don't change them):
 
https://github.com/alievk/avatarify-python/blob/master/docs/README.md#download-network-weights and place vox-adv-cpk.pth.tar file in the avatarify-python directory (don't unpack it).
Run run_windows.bat. If installation was successful, two windows "cam" and "avatarify" will appear. Leave these windows open for the next installation steps.

Install [VirtualCam plugin](https://obsproject.com/forum/resources/obs-virtualcam.539/). Choose Install and register only 1 virtual camera.
Run [OBS Studio](https://obsproject.com/).
In the Sources section, press on Add button ("+" sign), select Windows Capture and press OK. In the appeared window, choose "[python.exe]: avatarify" in Window drop-down menu and press OK. Then select Edit -> Transform -> Fit to screen.
In OBS Studio, go to Tools -> VirtualCam. Check AutoStart, set Buffered Frames to 0 and press Start.
Now OBS-Camera camera should be available in Zoom (or other videoconferencing software).
The steps 10-11 are required only once during setup.
