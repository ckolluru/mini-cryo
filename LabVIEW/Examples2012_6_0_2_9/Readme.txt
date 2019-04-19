Important Information On How The Example VIs Are Designed

The way the SITK(R) Vis gain access to a camera is through a camera handle.  The example VIs are designed to use a camera handle that exists as a global variable.  Thus the handle must be opened by running the ExOpenGlobalCam.vi (in the Open-Close folder) BEFORE running any example vi.  It need only be run once before using the examples.  When the work session is finished, the ExCloseGlobalCam.vi (also in the Open-Close folder) must be run to close out the camera, free up any buffers allocated and unload the SITK(R) dlls.
To reiterate,

   1) Open LabVIEW

   2) Run ExOpenGlobalCam.vi

   3) Do work (run and/or modify example vis, design new vis, etc.)

   4) Run ExCloseGlobalCam.vi

   5) Close LabVIEW
