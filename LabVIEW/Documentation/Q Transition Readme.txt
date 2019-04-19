SITIK Transition VI substitution for QCam VIs

The QCam to SITK Transition VIs have the same names and terminals as the old QCam Vis
and thus may directly replace them.

Here are some of the ways this can be done.
(Note: <LabVIEW_Folder> = C:\Program Files\National Instruments\LabVIEW XX where XX is the version)

1) Automatic Substitution from Renamed .llb File
     a) Locate the folder containing the old QCam.llb file
     b) Rename the old QCam.llb file to QCam_Old.llb
     c) If it is not already in the same folder, copy the SITK QI Transition library
        "<LabVIEW_Folder>/user.lib/QI_Transition.llb"to the same folder as the renamed
        QCam_Old.llb file.
     d) Rename the file "QI_Transition.llb" to "QCam.llb"
     e) Open your program to be updated.
     f) All the old QCam VIs will be replaced with the new SITK QI Transition VIs

2) Automatic Substitution from VIs in Memory :
     a) Create a new VI
     b) Add all the SITK QI Transition VIs from the SITK QI Transition VI library
        (<LabVIEW_Folder>/user.lib/QI_Transition.llb)
     c) Open your program to be updated
     d) LabVIEW will ask if you want to use the VIs already in memory.  Select "yes" or "ok".
     e) All QCam Vis will be replaced with SITK QI Transition VIs

3) Individual VI Substitution :
     a) Open your program to be updated
     b) Remove the old QCam VI
     c) Insert an SITK QI Transition VI of the same name from the SITK QI Transition VI library
        (<LabVIEW_Folder>/user.lib/QI_Transition.llb)
     d) Restore the wiring
