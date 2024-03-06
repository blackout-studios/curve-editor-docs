# CurveUndoStep
### Namespace: Blackout.UI


A custom undo type that handles animation curves


 ### Properties
| Type | Property Name | Accessor | Description |
| --- | --- | --- | --- |
 | `AnimationCurve` | Target | get; set;  | The target AnimationCurve |
 | [`AnimationCurveData`](../Data/AnimationCurveData.md) | Before | get; set;  | AnimationCurve data before changes |
 | [`AnimationCurveData`](../Data/AnimationCurveData.md) | After | get; set;  | AnimationCurve data after changes |

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | PerformUndo() | Applies the value of the before data to the animation curve |
| `void` | PerformRedo() | Applies the value of the after data to the animation curve |
| `void` | Free() | Free all the data used by this undo step back to the pool |
| `void` | RecordBefore() | Records the target animation curve to the before data |
| `void` | RecordAfter() | Records the target animation curve to the after data |
| [`CurveUndoStep`]() | Get() | Get a CurveUndoStep from the pool |
| `string` | ToString() |  |
