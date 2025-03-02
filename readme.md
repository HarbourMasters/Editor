# Editor

Editor that can interface with any port.

## How to make an object selectable in the editor
```
#include "Editor.h"
/**
  * model Provide the displaylist that contains vertices to setup accurate object selection
  * boundingBoxSize Set model to NULL and provide a boundingBoxSize to skip adding collision
 */
void AddObject(FVector* pos, Gfx* model, float scale, CollisionType collision, float boundingBoxSize)
```


# Setup
* Call Editor::Draw() at the end of the game draw code.
* Call Editor::Tick() at the end of the game ticking code.
* Call Editor::Load() near the start of game initialization.
