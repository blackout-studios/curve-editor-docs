# CurveScrollRect : UIBehaviour
### Namespace: Blackout.UI


An infinitely scrolling ScrollRect component that resizes itself to the position of the content. Contains logic for zooming and panning


 ### Serialized Fields

 | Type | Field Name | Description |
| --- | --- | --- |
| `RectTransform` | content |  |
| `RectTransform` | grid |  |
| `bool` | inertia |  |
| `float` | decelerationRate |  |
| `float` | zoomSensitivity |  |
| `float` | minimumZoom |  |
| `float` | maximumZoom |  |
| `RectTransform` | viewport |  |
| `Scrollbar` | horizontalScrollbar |  |
| `Scrollbar` | verticalScrollbar |  |
| `float` | horizontalScrollbarSpacing |  |
| `float` | horizontalScrollbarOffset |  |
| `float` | verticalScrollbarSpacing |  |
| [`AnimationCurveScrollRectEvent`](#AnimationCurveScrollRectEvent) | onPositionChanged |  |
| [`AnimationCurveScrollRectEvent`](#AnimationCurveScrollRectEvent) | onScaleChanged |  |


 ### Properties
| Type | Property Name | Accessor | Description |
| --- | --- | --- | --- |
 | `RectTransform` | Content | get; set;  |  |
 | `RectTransform` | Grid | get; set;  |  |
 | `bool` | Inertia | get; set;  |  |
 | `float` | DecelerationRate | get; set;  |  |
 | `float` | ZoomSensitivity | get; set;  |  |
 | `float` | MinimumZoom | get; set;  |  |
 | `float` | MaximumZoom | get; set;  |  |
 | `RectTransform` | Viewport | get; set;  |  |
 | `Scrollbar` | HorizontalScrollbar | get; set;  |  |
 | `Scrollbar` | VerticalScrollbar | get; set;  |  |
 | `float` | HorizontalScrollbarSpacing | get; set;  |  |
 | `float` | VerticalScrollbarSpacing | get; set;  |  |
 | [`AnimationCurveScrollRectEvent`](#AnimationCurveScrollRectEvent) | OnPositionChanged | get; set;  |  |
 | [`AnimationCurveScrollRectEvent`](#AnimationCurveScrollRectEvent) | OnScaleChanged | get; set;  |  |
 | `Vector2` | Velocity | get; set;  |  |
 | `Vector2` | NormalizedPosition | get; set;  |  |
 | `float` | HorizontalNormalizedPosition | get; set;  |  |
 | `float` | VerticalNormalizedPosition | get; set;  |  |
 | `float` | minWidth | get;  | Called by the layout system. |
 | `float` | preferredWidth | get;  | Called by the layout system. |
 | `float` | flexibleWidth | get;  | Called by the layout system. |
 | `float` | minHeight | get;  | Called by the layout system. |
 | `float` | preferredHeight | get;  | Called by the layout system. |
 | `float` | flexibleHeight | get;  | Called by the layout system. |
 | `int` | layoutPriority | get;  | Called by the layout system. |

 ### Methods
| Type | Method | Description |
| --- | --- | --- |
| `void` | Rebuild(CanvasUpdate executing) | Rebuilds the scroll rect data after initialization. |
| `void` | LayoutComplete() |  |
| `void` | GraphicUpdateComplete() |  |
| `bool` | IsActive() |  |
| `void` | StopMovement() | Sets the velocity to zero on both axes so the content stops moving. |
| `void` | ZoomToFit(float width, float height) |  |
| `void` | CalculateLayoutInputHorizontal() | Called by the layout system. |
| `void` | CalculateLayoutInputVertical() | Called by the layout system. |
| `void` | SetLayoutHorizontal() | Called by the layout system. |
| `void` | SetLayoutVertical() | Called by the layout system. |


# <a name="AnimationCurveScrollRectEvent">AnimationCurveScrollRectEvent</a> : UnityEvent<Vector2>
