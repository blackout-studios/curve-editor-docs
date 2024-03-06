# UndoHandler : MonoBehaviour
### Namespace: Blackout.UI


A generic undo/redo handler


 ### Public Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| `int` | maxSteps | The maximum number of undo steps to record |

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | AddStep(IUndoStep undoStep) | Record an undo step |
| `void` | PerformUndo() | Perform a undo step on the specified curve |
| `void` | PerformRedo() | Perform a redo step on the specified curve |
