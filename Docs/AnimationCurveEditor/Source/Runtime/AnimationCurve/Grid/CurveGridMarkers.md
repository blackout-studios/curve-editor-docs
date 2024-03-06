# CurveGridMarkers : MonoBehaviour
### Namespace: Blackout.UI


Creates and positions text objects in the correct place to line up with the grid


 ### Serialized Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| [`CurveScrollRect`](CurveScrollRect.md) | scrollRect |  |
| [`AnimationCurveEditor`](../AnimationCurveEditor.md) | editor |  |
| [`MovementDirection`](#MovementDirection) | direction | The direction to draw the value markers in. |
| [`GenericTextComponent`](../../Common/UI/GenericTextComponent.md) | template | The text template to use for the value markers. |
| `LabelSeparation[]` | labelSeparation | The separation between value markers at different scales. The scale is the scale of the content transform. The cells is the number of grid cells between each value marker. |


 ### Properties
| Type | Property Name | Accessor | Description |
| --- | --- | --- | --- |
 | [`CurveScrollRect`](CurveScrollRect.md) | ScrollRect | get; set;  |  |
 | [`AnimationCurveEditor`](../AnimationCurveEditor.md) | Editor | get; set;  |  |
 | [`MovementDirection`](#MovementDirection) | Direction | get; set;  |  |
 | [`GenericTextComponent`](../../Common/UI/GenericTextComponent.md) | Template | get; set;  |  |


# <a name="LabelSeparation">LabelSeparation</a>


 ### Public Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| `float` | scale |  |
| `float` | cells |  |


# <a name="MovementDirection">MovementDirection</a> : Enum
| Name | Description |
| --- | --- |
| Horizontal |  |
| Vertical |  |
