# Animation Curve Button
<img src = "https://i.gyazo.com/c671461fec8145296b3316cfd05a593d.png"/>
The animation curve button is a simple button with a renderer to render the animation curve. It is what you will use in your user interface that will allows users to open the curve editor.
<br>
<br>

**Adding a button to your scene**
<br>

You can add a *Animation Curve Button* to your scene via the asset menu.
<br>
<img src="https://i.gyazo.com/2f5b837a152e2a74ee2cf6d8b50357bd.png" width="300"/><br>
<img src="https://i.gyazo.com/1da02871f4e4644121b46c2f061baf76.png" width="300"/>
<br>

Upon first adding an Animation Curve Button to your scene, the scene will be checked to see if a *Animation Curve Editor* already exists. If not, you will be asked if you would like to generate one.
<br>
<img src="https://i.gyazo.com/0562b10f39a0baa4567eb30c6d6c9133.png" width="400"/>
<br>

This step is not essential, it only asks so it can automatically assign a editor reference to the button when it is generated. If you opt not to add a *Animation Curve Editor* at this stage, you will need to manually assign the editor reference later.<br>
<img src="https://i.gyazo.com/4ee325561b1bec6b8f1eaf068ccb8fc2.png" width="400"/>
<br>
<br>

**Assigning a curve to the AnimationCurveButton component**
<br>

The **AnimationCurveButton** component will already be present on the button when you generate it. Assigning a curve to the button is the only essential coding you will need to do in order to use the *Animation Curve Editor*.
<br>

To assign a curve to the button from your code that is using the *AnimationCurve*, you will first need to add a reference to the *AnimationCurveButton* component in your script.
<br>

Then at any some stage during the components initialization assign your *AnimationCurve* instance to the *Curve* property of the *AnimationCurveButton*

```csharp
using Blackout.UI;
using UnityEngine;

public class ExampleScript : MonoBehaviour
{
    [SerializeField]
    private AnimationCurve myCurveReference;
    
    [SerializeField]
    private AnimationCurveButton animationCurveButton;

    private void Start()
    {
        animationCurveButton.Curve = myCurveReference;
    }
}
```

Once you have assigned an AnimationCurve to the *Animation Curve Button* that curve instance will be the only instance edited when the user presses the button unless a different curve instance is assigned to it.<br>
As a AnimationCurve is a reference type, there is no need for you to retrieve the instance after changes have been made to it.
