# CurveKeyframe : MonoBehaviour
### Namespace: Blackout.UI


The class that controls manipulation of keyframes on the grid


 ### Serialized Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| `Image` | handle |  |
| [`CurveTangent`](CurveTangent.md) | leftTangent |  |
| [`CurveTangent`](CurveTangent.md) | rightTangent |  |


 ### Public Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| [`AnimationCurveEditor`](../AnimationCurveEditor.md) | editor |  |
| `int` | _keyframeIdx |  |


 ### Properties
| Type | Property Name | Accessor | Description |
| --- | --- | --- | --- |
 | `Keyframe` | Keyframe | get; set;  |  |
 | [`KeyframeData`](../Data/KeyframeData.md) | Data | get; set;  |  |
 | `int` | KeyframeIndex | get; set;  |  |
 | `float` | Time | get; set;  |  |
 | `float` | Value | get; set;  |  |
 | `bool` | BrokenTangents | get; set;  |  |
 | `Image` | Handle | get; set;  |  |
 | [`CurveTangent`](CurveTangent.md) | LeftTangent | get; set;  |  |
 | [`CurveTangent`](CurveTangent.md) | RightTangent | get; set;  |  |
 | [`AnimationCurveEditor`](../AnimationCurveEditor.md) | Editor | get; set;  |  |

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | Select() | Select this keyframe |
| `void` | Deselect() | Deselect this keyframe |
| `void` | FinalizeUpdate() | Updates keyframe data and surrounding tangents and sends the data back to the editor |
| `void` | SetBrokenTangents(bool v) | Marks the tangents as broken so they can be moved individually |
| `void` | SetFlattenTangents() | Flatten the tangents |
| `void` | SetBothTangents(TangentMode mode, bool sendUpdate) | Set tangent mode for both sides and update accordingly |
| `void` | SetSideTangent(bool isLeft, TangentMode mode) | Set the tangent mode for one side and update accordingly |
| `void` | UpdateTangentData(CurveTangent tangent, int tangentMode) | Set the tangent mode and rotation from the tangent handle. |
