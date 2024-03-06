# TangentToggleButton : [`TangentHoverColorTransition`](TangentHoverColorTransition.md)
### Namespace: Blackout.UI


Custom toggle used in the tangent menu


 ### Serialized Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| `bool` | isOn | Is the toggle currently on or off? |
| `Graphic` | graphicBox |  |
| `Graphic` | graphicCheckmark |  |
| [`ToggleEvent`](#ToggleEvent) | onValueChanged |  |


 ### Properties
| Type | Property Name | Accessor | Description |
| --- | --- | --- | --- |
 | `bool` | IsOn | get; set;  |  |
 | [`ToggleEvent`](#ToggleEvent) | OnValueChanged | get; set;  |  |
 | `Graphic` | GraphicBox | get; set;  |  |
 | `Graphic` | GraphicCheckmark | get; set;  |  |

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | SetIsOnWithoutNotify(bool value) |  |
| `void` | OnPointerClick(PointerEventData eventData) |  |
| `void` | OnPointerDown(PointerEventData eventData) |  |


# <a name="ToggleEvent">ToggleEvent</a> : UnityEvent<bool>
