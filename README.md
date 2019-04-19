# mini-cryo
LabVIEW code to operate the mini-cryo system.

All changes to the backup copy of 9/6/18 will be documented henceforth to ensure reproducibility.

1. Renamed "mainCryo With New Driver V1 and Cri Modified by Patiwet.vi" to "mainCryo.vi" (Makes it simpler to use).

2. mainCryo.vi and QCam Color Snap.vi had their dependencies from older folders and are now loaded from this local folder. Labview raises 5 warnings, all ignored.

3. If the camera is not switched on and the Labview program is run, you will get an error saying that another program is using the camera.
The New Camera folder seems to have all the subVIs necessary for the camera. A lot of the block VI for QCamera_V1.0 is similar to mainCryo.vi

4. C:\Program Files\National Instruments\LabVIEW 2012\user.lib\QI_Transition.llb has a bunch of VIs which do multiple options for the VI.
Here are all the VIs in this llb file.

![alt text](https://user-images.githubusercontent.com/8373968/45765273-a50f4d00-bc02-11e8-84ef-2ec4e15c9146.png)

5.
