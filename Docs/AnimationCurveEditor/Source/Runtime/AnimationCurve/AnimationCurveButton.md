# AnimationCurveButton : Selectable
### Namespace: Blackout.UI


A custom button that draws a animation curve, and opens the editor when clicked.


 ### Serialized Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| `AnimationCurve` | curve |  |
| [`ButtonCurveRenderer`](Renderers/ButtonCurveRenderer.md) | curveRenderer |  |
| [`CurveUpdateMode`](#CurveUpdateMode) | updateMode | When to update this components curve renderer with changes from the editor. |
| [`AnimationCurveEditor`](AnimationCurveEditor.md) | editor |  |


 ### Properties
| Type | Property Name | Accessor | Description |
| --- | --- | --- | --- |
 | `AnimationCurve` | Curve | get; set;  |  |
 | [`CurveRenderer`](Renderers/CurveRenderer.md) | CurveRenderer | get; set;  |  |
 | [`CurveUpdateMode`](#CurveUpdateMode) | UpdateMode | get; set;  |  |
 | [`AnimationCurveEditor`](AnimationCurveEditor.md) | Editor | get; set;  |  |
 | [`AnimationCurveEvent`](#AnimationCurveEvent) | OnClick | get; set;  |  |
 | `bool` | OverrideOnClick | get; set;  | If true, the OnClick event will be invoked instead of the button press defaulting to opening the curve editor and editing the curve |


# <a name="AnimationCurveEvent">AnimationCurveEvent</a> : UnityEvent<AnimationCurve>


# <a name="CurveUpdateMode">CurveUpdateMode</a> : Enum
Determines at what point the button renderer should update when using the editor.
| Name | Description |
| --- | --- |
| None | Never updates (useful for curve presets as they never change) |
| OnUpdate | Updates the button renderer every frame when the curve in the editor has changed |
| OnEndEdit | Updates the button renderer when the editor has been closed |
