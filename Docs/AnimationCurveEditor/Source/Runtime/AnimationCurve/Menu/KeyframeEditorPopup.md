# KeyframeEditorPopup : MonoBehaviour
### Namespace: Blackout.UI


Controller for the keyframe editor popup


 ### Serialized Fields

 **Curve Buttons**

 | Type | Field Name | Description |
| --- | --- | --- |
| [`TangentMenuButton`](TangentMenuButton.md) | deleteButton |  |
| [`TangentMenuButton`](TangentMenuButton.md) | editButton |  |
| [`TangentToggleButton`](TangentToggleButton.md) | clampedAutoToggle |  |
| [`TangentToggleButton`](TangentToggleButton.md) | autoToggle |  |
| [`TangentToggleButton`](TangentToggleButton.md) | flatToggle |  |
| [`TangentToggleButton`](TangentToggleButton.md) | freeSmoothToggle |  |
| [`TangentToggleButton`](TangentToggleButton.md) | brokenToggle |  |
| [`TangentFoldoutButton`](TangentFoldoutButton.md) | leftTangentButton |  |
| [`TangentFoldoutButton`](TangentFoldoutButton.md) | rightTangentButton |  |
| [`TangentFoldoutButton`](TangentFoldoutButton.md) | bothTangentButton |  |

 **Tangent Sub Menu**

 | Type | Field Name | Description |
| --- | --- | --- |
| `GameObject` | tangentMenu |  |
| [`TangentToggleButton`](TangentToggleButton.md) | tangentFreeToggle |  |
| [`TangentToggleButton`](TangentToggleButton.md) | tangentLinearToggle |  |
| [`TangentToggleButton`](TangentToggleButton.md) | tangentConstantToggle |  |
| [`TangentToggleButton`](TangentToggleButton.md) | tangentWeightedToggle |  |


 ### Public Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| [`AnimationCurveEditor`](../AnimationCurveEditor.md) | editor |  |


 ### Properties
| Type | Property Name | Accessor | Description |
| --- | --- | --- | --- |
 | [`TangentMenuButton`](TangentMenuButton.md) | DeleteButton | get; set;  |  |
 | [`TangentMenuButton`](TangentMenuButton.md) | EditButton | get; set;  |  |
 | [`TangentToggleButton`](TangentToggleButton.md) | ClampedAutoToggle | get; set;  |  |
 | [`TangentToggleButton`](TangentToggleButton.md) | AutoToggle | get; set;  |  |
 | [`TangentToggleButton`](TangentToggleButton.md) | FlatToggle | get; set;  |  |
 | [`TangentToggleButton`](TangentToggleButton.md) | FreeSmoothToggle | get; set;  |  |
 | [`TangentToggleButton`](TangentToggleButton.md) | BrokenToggle | get; set;  |  |
 | [`TangentFoldoutButton`](TangentFoldoutButton.md) | LeftTangentButton | get; set;  |  |
 | [`TangentFoldoutButton`](TangentFoldoutButton.md) | RightTangentButton | get; set;  |  |
 | [`TangentFoldoutButton`](TangentFoldoutButton.md) | BothTangentButton | get; set;  |  |
 | `GameObject` | TangentMenu | get; set;  |  |
 | [`TangentToggleButton`](TangentToggleButton.md) | TangentFreeToggle | get; set;  |  |
 | [`TangentToggleButton`](TangentToggleButton.md) | TangentLinearToggle | get; set;  |  |
 | [`TangentToggleButton`](TangentToggleButton.md) | TangentConstantToggle | get; set;  |  |
 | [`TangentToggleButton`](TangentToggleButton.md) | TangentWeightedToggle | get; set;  |  |

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | SetKeyframe(CurveKeyframe keyframe) |  |
| `void` | OpenTangentMenu(RectTransform rectTransform, Side side) |  |
| `void` | CloseTangentMenu(Side side) |  |
