# CurveEditorSettings : ScriptableObject
### Namespace: Blackout.UI


Contains all the visual data of the curve editor in one place


 ### Public Fields

 **Keyframes**

 | Type | Field Name | Description |
| --- | --- | --- |
| `Color` | keyframeDeselectedColor | The color of a deselected keyframe node |
| `Color` | keyframeSelectedColor | The color of a selected keyframe node |

 **Grid Render**

 | Type | Field Name | Description |
| --- | --- | --- |
| `Color` | gridPrimaryColor | The color of the main lines of the grid. These are the lines located on whole numbers |
| `Color` | gridSecondaryColor | The color of the secondary lines of the grid |
| `float` | gridLineThickness | The pixel thickness of the rendered grid |
| `int` | gridPixelsPerCell | The number of pixels per grid cell |

 **Curve Render**

 | Type | Field Name | Description |
| --- | --- | --- |
| `Color` | curveColor | The color of the rendered curve |
| `float` | curveThickness | The pixel thickness of the rendered curve |
| `float` | curveClickThickness | The thickness in pixels around the line that are determined to be valid clicks |
| `float` | curveDoubleClickTime | The thickness in pixels around the line that are determined to be valid clicks |

 **Keyframe Editor Popup**

 | Type | Field Name | Description |
| --- | --- | --- |
| `Color` | keyframeEditorButtonColor | The hover color of the buttons in the keyframe editor popup |
| `float` | keyframeEditorButtonFadeDuration | The fade duration of the buttons in the keyframe editor popup |

 **Presets**

 | Type | Field Name | Description |
| --- | --- | --- |
| `List<AnimationCurve>` | curvePresets | The default curve presets that are loaded when the editor is opened |
