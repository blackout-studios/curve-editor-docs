# KeyframeData
### Namespace: Blackout.UI


A serializable data class that represents a Keyframe


 ### Public Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| `float` | time | The time of the keyframe |
| `float` | value | The value of the curve at keyframe |
| `float` | inTangent | Sets the incoming tangent for this key. The incoming tangent affects the slope of the curve from the previous key to this key |
| `float` | outTangent | Sets the outgoing tangent for this key. The outgoing tangent affects the slope of the curve from this key to the next key |
| `float` | inWeight | Sets the incoming weight for this key. The incoming weight affects the slope of the curve from the previous key to this key |
| `float` | outWeight | Sets the outgoing weight for this key. The outgoing weight affects the slope of the curve from this key to the next key |
| `WeightedMode` | weightedMode | Weighted mode for the keyframe |
| `int` | tangentMode |  |

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | CopyFrom(Keyframe keyframe) | Copies a keyframes data to this data structure |
