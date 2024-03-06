# AnimationCurveEditor : MonoBehaviour
### Namespace: Blackout.UI


The main class of the curve editor. This class handles all the individual components used for editing curves


 ### Serialized Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| [`CurveEditorSettings`](Data/CurveEditorSettings.md) | settings | A curve settings asset that contains all the settings for the curve editor |

 **Curve**

 | Type | Field Name | Description |
| --- | --- | --- |
| `AnimationCurve` | curve | The curve to edit. This should be set via code when opening the curve editor |
| `bool` | clampCurve | When enabled, each keyframes time and value components will be clamped between 0.0 and 1.0 |

 **Components**

 | Type | Field Name | Description |
| --- | --- | --- |
| [`GenericTextComponent`](../Common/UI/GenericTextComponent.md) | windowTitle | Reference to the window title generic text component |
| [`CurveScrollRect`](Grid/CurveScrollRect.md) | scrollRect |  |
| [`CurveGrid`](Grid/CurveGrid.md) | curveGrid |  |
| [`GridCurveRenderer`](Renderers/GridCurveRenderer.md) | curveRenderer |  |
| [`KeyframeEditorPopup`](Menu/KeyframeEditorPopup.md) | keyframeEditor | Reference to the keyframe tangent editor popup |
| `GameObject` | curveQuickActions | Reference to the quick action menu popup |
| [`UndoHandler`](../Common/Undo/UndoHandler.md) | undoHandler | Reference to the UndoHandler component |

 **Keyframes**

 | Type | Field Name | Description |
| --- | --- | --- |
| [`CurveKeyframe`](Keyframes/CurveKeyframe.md) | keyframeTemplate | Reference to the keyframe template object |
| `GameObject` | keyframeValues | Reference to the keyframe values popup |
| `Vector2` | valueInputOffset | The distance away from the keyframe marker the input and value fields will be placed |
| [`GenericInputComponent`](../Common/UI/GenericInputComponent.md) | timeInput | Reference to the time generic input component in the keyframe values popup |
| [`GenericInputComponent`](../Common/UI/GenericInputComponent.md) | valueInput | Reference to the value generic input component in the keyframe values popup |

 **Presets**

 | Type | Field Name | Description |
| --- | --- | --- |
| [`AnimationCurveButton`](AnimationCurveButton.md) | presetTemplate | Reference to the preset template button |


 ### Properties
| Type | Property Name | Accessor | Description |
| --- | --- | --- | --- |
 | [`GenericTextComponent`](../Common/UI/GenericTextComponent.md) | WindowTitle | get; set;  |  |
 | `AnimationCurve` | Curve | get; set;  |  |
 | [`UndoHandler`](../Common/Undo/UndoHandler.md) | UndoHandler | get; set;  |  |
 | [`CurveEditorSettings`](Data/CurveEditorSettings.md) | Settings | get; set;  |  |
 | [`CurveScrollRect`](Grid/CurveScrollRect.md) | ScrollRect | get; set;  |  |
 | [`GridCurveRenderer`](Renderers/GridCurveRenderer.md) | CurveRenderer | get; set;  |  |
 | [`CurveKeyframe`](Keyframes/CurveKeyframe.md) | KeyframeTemplate | get; set;  |  |
 | [`CurveGrid`](Grid/CurveGrid.md) | Grid | get; set;  |  |
 | `GameObject` | KeyframeValuesPopup | get; set;  |  |
 | [`KeyframeEditorPopup`](Menu/KeyframeEditorPopup.md) | KeyframeEditor | get; set;  |  |
 | `GameObject` | CurveQuickActions | get; set;  |  |
 | [`GenericInputComponent`](../Common/UI/GenericInputComponent.md) | TimeInput | get; set;  |  |
 | [`GenericInputComponent`](../Common/UI/GenericInputComponent.md) | ValueInput | get; set;  |  |
 | [`AnimationCurveButton`](AnimationCurveButton.md) | PresetTemplate | get; set;  |  |
 | `bool` | ClampCurve | get; set;  |  |
 | `int` | KeyframeCount | get;  |  |

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | EditCurve(AnimationCurve animationCurve) | Opens the editor and sets the curve to edit |
| `void` | GetCurveRange(out Vector2 min, out Vector2 max) | Get the min/max range of the curve |
| [`CurveKeyframe`](Keyframes/CurveKeyframe.md) | GetKeyframe(int idx) | Get the keyframe at the specified index |
| `bool` | CanInsertAtTime(float time) | Check if the time is between the start and end keyframes |
| `void` | InsertKeyframe(float time, float value) | Insert a keyframe the the specified time and value |
| `void` | SelectKeyframe(CurveKeyframe keyframe) | Sets the selected keyframe and deselects the previous one |
| `void` | DeselectKeyframe(CurveKeyframe keyframe) | De-select the specified keyframe, if it is selected |
| `bool` | IsSelectedKeyframe(CurveKeyframe keyframe) | Check if the specified keyframe is selected |
| `void` | UpdateKeyframe(CurveKeyframe keyframe) | Update the keyframe in the curve and redraw the curve. |
| `void` | UpdateCurve() | Redraws the curve and send out the onValueChanged event. |
| `void` | DeleteKeyframe(CurveKeyframe keyframe) | Delete the specified keyframe from the curve |
| `Vector2` | ConvertNormalizedToCurveRange(Vector2 input) | Converts a normalized input to the range of the curve |
| `void` | ToggleKeyframeValuesPopup(bool active) | Toggle the keyframe values popup and position it relative to the selected keyframe. |
| `void` | OpenKeyframeEditor(CurveKeyframe keyframe) | Open the keyframe editor popup |
| `void` | AddPreset(AnimationCurve animationCurve) | Add a AnimationCurve preset to the editor |
| `void` | RecordState(bool finalize) | Record the current state of the curve |
| `void` | RebuildCurve() | Recycles all the curve components and rebuild it |


# <a name="AnimationCurveEvent">AnimationCurveEvent</a> : UnityEvent<AnimationCurve>
