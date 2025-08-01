Changelog
#########

v0.1.7
======

Improvements
~~~~~~~~~~~~
* The addon got a major code rework to ensure stablility and improve performance.
* Compatibility with 3.6 LTS, 4.2 LTS and later version.

Changes
~~~~~~~
* Flat variants won't need a second click to finalize the object.
* Working plane position won't reset when changing the size.

Fixes
~~~~~
* Object may not initialized completly for the raycast.
* Fix the width of the line while settings the segments count.


v0.1.61
=======

Improvements
~~~~~~~~~~~~
* Numpad keys are usable from the addon to change the camera view

Fixes
~~~~~
* -Y orthographic view crash
* Changing smoothing while creating objects crash


v0.1.6
======

Improvements
~~~~~~~~~~~~
* Ignore objects with wireframe or bound viewport display
* Hide the UI block next to the mouse cursor with F2
* 3D cursor set to the working plane center

Changes
~~~~~~~
* F1 and F2 keys change the addon preference values directly

Fixes
~~~~~
* Height increment with shift key can stuck
* Raycast can fail and crash the addon in some cases

v0.1.54
=======
Fixes
~~~~~
* Blender 4.1 compatibility fix.

Improvements
~~~~~~~~~~~~
* UV map channel created for objects


v0.1.53
=======
Fixes
~~~~~
* Blender 4.0 compatibility fix.


v0.1.51
=======
Fixes
~~~~~
* Fix inverted normals issue.
* Blender 2.91 compatibility fix.


v0.1.5
======
New features
~~~~~~~~~~~~
* Convert to qblock tool.
* Edit mode object creation.
* Sphere cube and Corner cube objects.
* Grid hit only option. **E**
* Change working plane size. **CTRL+W**
* Snapping turning off in height stage. (Can change in preferences.)

Improvements
~~~~~~~~~~~~
* Change mesh and snap segments with the same key for mouse scroll and pen move.
* Help section improvements. Toggle with **F1**.
* Lots of code simplifications and optimization.
* Plane and Circle QObject merged into the Cube and Cylinder objects with the Flat parameter.

Fixes
~~~~~
* Segments slider number at the start position to avoid going offscreen.
* Snap subdivision generates subpoints on grid edges too.
* Uniform scale object creation wait for another mouse click to allow changing the segments.
* Setting the Cylinder and Sphere radius to 0 crashes the tool.
* Cylinder depth parameter now in world unit.

v0.1.4
======
* Additional addon settings for colors and scales.
* New option to ignore mesh behind the grid with **E** key.
* Parametric objects.
* QBlocker panel removed from the context menu.

v0.1.3
======
* Default segments count in preferences.
* The closest snap point is now calculated by distance.
* Snap variations now mapped to **Y(Z)** and **X** keys.
* Change snap subdivision can be changed by holding the **C** key and using the mouse wheel.
* Creating object in **local view** now remain visible.
* **BaseTypes** now can be set with the ctrl and shift keys.
* New **Turn into Cylinder** tool.

v0.1.2
======
* **Axis and Oriented** coordinate systems.
* **Working Space** feature.
* Axis orientation is now aligned to Blender World.
* Optional Hold or Toggle settings for snap-in preferences.
* High-resolution text row gap fixed.
* New object created into the active collection.

v0.1.1
======
* Add **Plane** and **Circle** mesh alternatives for operators.
* **"Resolution Scale"** in **"Preferences"** now affect addon ui text size.
* Snap points can now be generated on objects with modifiers.
* Activate Snap remapped to **'CTRL'** key to avoid Maya like camera control.
* Exiting addon while creating mesh now deletes unfinished objects.
* Tweak segments when holding **'S'** now locks mesh height.
* Shader Compile Error fixed.
* Addon has a unique preference for select_mouse to avoid custom keymap issues.