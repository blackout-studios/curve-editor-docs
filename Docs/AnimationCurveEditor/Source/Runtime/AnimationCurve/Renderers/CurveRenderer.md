# CurveRenderer : MaskableGraphic
### Namespace: Blackout.UI


The curve renderer base class holds all of the common logic used by the different curve renderers


 ### Serialized Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| `RectTransform` | content |  |
| `AnimationCurve` | curve |  |
| `bool` | isDirty |  |
| `UIVertex` | vertex |  |
| `Vector2` | minRange |  |
| `Vector2` | maxRange |  |


 ### Properties
| Type | Property Name | Accessor | Description |
| --- | --- | --- | --- |
 | `Vector2` | MinRange | get;  |  |
 | `Vector2` | MaxRange | get;  |  |
 | `bool` | HasCurve | get;  |  |
 | `RectTransform` | Content | get; set;  |  |
 | `AnimationCurve` | Curve | get; set;  |  |

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | MarkDirty() | Mark the curve dirty so it will be recalculated |
| `void` | Redraw() | Redraws the curve without recalculating the curve itself |
| `void` | SetCurve(AnimationCurve animationCurve) | Set the curve to be rendered |
