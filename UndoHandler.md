# Undo Handler

The undo handler records changes you make to the curve via the editor.<br>

You can undo/redo changes using the buttons in the top right of the editor screen.<br>
<img src="https://i.gyazo.com/3dcccd9cd487fac2b4c39674072048fa.png" width="400"/>
<br>

The component itself lives on the *Animation Curve Editor* object in your scene.<br>
It only has 1 configurable option and that is the number of undo steps it can record.<br>
When it reaches the max number of steps it will start removing the steps from the beginning of the list
<img src="https://i.gyazo.com/988ea9fb4fa8f8de3dc854ce48930182.png" width="400"/><br>

While no hotkeys have been implemented to perform undo/redo actions by default, such can easily be implemented youself using the provided API<br>

[UndoHandler API Reference](Docs/AnimationCurveEditor/Source/Runtime/Common/Undo/UndoHandler.md)