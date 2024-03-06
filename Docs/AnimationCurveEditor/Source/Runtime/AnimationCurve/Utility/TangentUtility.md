# TangentUtility
### Namespace: Blackout.UI

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | DecodeTangents(int tangentMode, out TangentMode left, out TangentMode right) | Decode the tangent mode into left and right tangent modes. |
| `int` | EncodeTangents(TangentMode mode) | Encode the specified tangent mode on to both side into a single integer. |
| `int` | EncodeTangents(TangentMode left, TangentMode right) | Encode the left and right tangent modes into a single integer. |
| `float` | TangentToDegrees(float t) | Convert a tangent to degrees. |
| `float` | DegreesToTangent(float d) | Convert degrees to a tangent. |
| `Quaternion` | TangentToRotation(float t) | Convert a tangent to a rotation suitable for the keyframe UI. |
