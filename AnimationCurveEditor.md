# Animation Curve Editor
The animation curve editor is what you will use to manipulate an animation curve.
<br>

Note: You only need 1 instance of the *Animation Curve Editor* in your scene.
<br>

**Adding a editor to your scene**
<br>

You can add a *Animation Curve Editor* to your scene via the asset menu.
<br>
<img src="https://i.gyazo.com/0910dce273143b85aee125557a570631.png" width="300"/><br>
<img src="https://i.gyazo.com/bb6d7bfe488a34261d5b53a8e5a5811a.png" width="300"/>
<br>

When you first generate a instance of the *Animation Curve Editor* in your project, a instance of the *[Curve Editor Settings](Docs/AnimationCurveEditor/Source/Runtime/AnimationCurve/Data/CurveEditorSettings.md)* scriptable object will be generated and placed in your resources folder.<br>
<img src="https://i.gyazo.com/f0dfb1873b0e24f3c17eae91e3dffff6.png" width="600"/><br>
<img src="https://i.gyazo.com/4c4d34eefdebabd2d15f979add1ae10e.png" width="600"/><br>
This object contains the default settings for the curve editor. These settings are used across many components that make up the curve editor, so having this ScriptableObject is just for the convenience of having all these options in 1 central location.<br>



