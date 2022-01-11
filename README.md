# Light Object Tracker

Unreal Engine project demonstraing how we can track and object with a spotlight.

## Usage
There's a Spot Light and a Target Point in the level. Drag the target point in the editor and see how the spotlight follows it. Likewise, drag the spotlight around and see how it keeps pointing at the target point. This is useful if you want to setup portrait lighting in the Unreal Editor, with no intention of ever "playing" the game. 

## How does this black magic work?
The project relies on the implementation of an Editor Tick event so that the rotation of the spotlight can be continously updated. The regular Tick event is only available when we play the project, but not in the Editor. Here's how the Editor Tick is implemented: https://github.com/versluis/EditorTicker
