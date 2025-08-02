Changelog
#########

v0.2.2
======
New features
~~~~~~~~~~~~
* Optional slice parameters for all cylindrical objects.
* Working plane now using an endless grid.
* Cube object got a taper parameter.
* Close caps parameter for Tube object.
* The mesh generators now set custom sharp edges for all objects.

Improvements
~~~~~~~~~~~~
* The addon got a major code rework to ensure stablility and improve performance.
* Compatibility with 3.6 LTS, 4.2 LTS and later version.
* Working plane can use the new UBO shader variant to run better on the latest versions. (and starting to support changes coming with the 5.0)

Changes
~~~~~~~
* Working plane position won't reset when changing the size.
* Flat variants won't need a second click to finalize the object.
* Pyramid object is now using the cube generator with a maximum taper parameter.

Fixes
~~~~~
* Object may not initialized completly for the raycast.
* Fix capsule zero height bug.
* Fix the width of the line while settings the segments count.

v0.2.1
======
New features
~~~~~~~~~~~~
* New mesh generators
* Flat mesh variant for tube
* UV generated for all object types
* Additional subdivision options for all object types
* UV stretch option for cylindrical objects
* Quick object type switch with 1-5 keys

Improvements
~~~~~~~~~~~~
* Qblocker converter ui fixed and updated to better mirror the object properties
* Numpad keys are usable from the addon to change the camera view

Changes
~~~~~~~
* Qblocker tools moved to a submenu in the object menu

Fixes
~~~~~
* -Y orthographic view crash
* Changing smoothing while creating objects crash

v0.2
====
New features
~~~~~~~~~~~~
* Capsule, Cone, Tube and Torus objects
* Active object instancing with new placement methods
* Set qobject base origin (new operator)
* floater window for quick qobject parameters (new operator)
* Customize hotkeys in addon preferences (WIP)
* Extra step for the object creation to handle secondary radius

Improvements
~~~~~~~~~~~~
* Ignore objects with wireframe or bound viewport display
* Hide the UI block next to the mouse cursor with F2
* 3D cursor set to the working plane center
* Unify UI scaling across the addon (WIP)
* Additional parameters in addon preferences

Changes
~~~~~~~
* F1 and F2 keys change the addon preference values directly
* With the new origin set operator Corner Cube has become obsolete (still exists in the code, but removed from UI)
* The torus object is temporarily removed from the addon.

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
* Uniform scale object creation waits for another mouse click to allow changing the segments.
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
* Optional Hold or Toggle settings for snap in the preferences.
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