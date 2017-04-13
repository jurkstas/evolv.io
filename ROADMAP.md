### Brain
Move the brain implementation more towards an OOP style. Currently the brain is a raw 3d array of a fixed length, this needs to be more flexible so that it is possible for brains to evolve over time.

### Rendering
Separate the rendering out from the updating using the Renderer interface. Currently rendering and updating is all mixed together. It would be nice to keep them separate so that the performance and correctness of updating isn't affected by the rendering.

### A more OOP UI
Currently user interaction is calculated by mouse position. There may need to be a concept of a UI button that can register responses to clicks. These buttons could be held in a HUD graph which allows interrogating which button is underneath any (x, y) co-ordinate.

### A scene graph
It would be nice for tiles and creatures to be held in a scene graph which allows objects to be added and removed. This scene graph might be a quadtree which would allow interrogating what was underneath any (x, y) co-ordinate in the same way as the ui/hud graph.

### Cleanup, efficiency
Some methods are still doing unusual things or could be improved, any improvements along these lines are helpful. The unusual methods may need some discussion about how to change them or whether to replace them.
