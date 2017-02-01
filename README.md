# Medientheater
The Unity basis setup for media theater projects.

## Instructions for v2
Here's the first update of the Unity setup. Just replace the old prefab with the new one. The assignment of the cameras in the scene to the projectors in the real world should now be correct.

What's still missing is the calibration of the cameras. The projections are still overlapping, but you can finally start working in the media theater. I will update the prefab again when calibration is done. 


## Instructions for v1
Advised setup:
 - Create a new scene in Unity (or use an existing one at your own risk ;)).
 - Double-click the .unitypackage file and confirm the import dialog (or right-click in your project structure view, select "Import Package"->"Custom Package..." and then choose the .unitypackage file).
 - Drag the "Medientheater" prefab to your scene.
 - Make sure that the transform is at (0, 0, 0).

Some annotations:
1. The dimensions are based on the SketchUp file in the classroom.
2. The cameras in the scene are not properly aligned, yet. Especially if the projectors don't project on the complete surface of the walls, the alignment may be completely wrong. Also, the assignment of the cameras to the projectors needs verification.
3. For both cases, I prepared some calibration support in form of the "Calibration" game object. I strongly advise you to read the comments in the script file.
4. If we all base our projects on this template, then only one group needs to struggle with the calibration and we can all profit by the shared camera settings. 
5. The other script ("Activate Displays" game object) can be used when building your project. It takes care of making Unity use more than one display. This does not work in testing mode, at least as far as I know. Again, mind the comments in the script file. 
