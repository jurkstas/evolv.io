### Brain
In progress

Move the brain implementation more towards an OOP style. Currently the brain is a raw 3d array of a fixed length, this needs to be more flexible so that it is possible for brains to evolve over time.

### Rendering
Renderer interface done, still a lot remaining to do

Separate the rendering out from the updating using the Renderer interface. Currently rendering and updating is all mixed together. It would be nice to keep them separate so that the performance and correctness of updating isn't affected by the rendering.

### A more fluid, responsive and OOP UI
TODO

Currently user interaction is calculated by comparing mouse positions against hard-coded values. The values need to be more responsive to screen size. Also there may need to be a concept of a UI button that can register responses to clicks. These buttons could be held in a HUD graph which allows interrogating which button is underneath any (x, y) co-ordinate.

### A scene graph
TODO

It would be nice for tiles and creatures to be held in a scene graph which allows objects to be added and removed. This scene graph might be a quadtree which would allow interrogating what was underneath any (x, y) co-ordinate in the same way as the ui/hud graph.

### A Plant SoftBody
TODO

At the moment there is currently just "grass" and Creatures. It would be nice to have a plant softbody too with it's own evolutionary cycles.

### Cleanup, efficiency, performance and more OOP style
A lot of clean up done, some efficiency work done, rendering performance needs to be looked at, OOP style is in progress.

Some methods are still doing unusual things or could be improved, any improvements along these lines are helpful. The unusual methods may need some discussion about how to change them or whether to replace them.
Efficiency still needs some work, eg. using squared distances instead of radius.
Performance needs looking at, especially what is being rendered.
Code concepts still need to be fully separated out and moved more towards an OOP style.
