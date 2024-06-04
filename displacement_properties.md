# Displacement Properties

- [Displacement Properties](#displacement-properties)
  - [Properties](#properties)
  - [Keywords](#keywords)
    - [DISPLACEMENT](#displacement)

## Properties
| Name                     | Type        | Default Value | Description                                                                                                                                                                                                  |
| ------------------------ | ----------- | ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| DisplaceMap              | Texture     | grey          | Displacement map, greyscale texture, ***red*** channel is used.                                                                                                                                              |
| DisplaceMiddleLevel      | Float(0,1)  | 0.5           | Define the non-displacement value on `DisplaceMap`. Any lower values will push the surfaces inwards, and any higher values will push them outwards. Typically, this value is middle grey (0.5) or black (0). |
| DisplaceStrength         | Float(0,1)  | 1             | The intensity of displacement application.                                                                                                                                                                   |
| DisplaceNormalMultiplier | Float(0,10) | 1             | Control the scale of the normals generated from `DisplaceMap`, used to adjust the surface normals after displacement. Works with `DisplaceStrength`.                                                         |
| DisplaceAdjustment       | Float(-1,1) | 0             | Extrude or intrude the displaced object along its normals with additional distance. This is an adjustment to the baseline of the displacement.                                                               |
| DisplaceOffset           | Vector      | (0,0,0,0)     | Offset the displaced object in its object space. ***red***: x-axis, ***green***: y-axis, ***blue***: z-axis, ***alpha***: not used.                                                                          |

## Keywords

### DISPLACEMENT
**Off**: Disable the displacement. ***Default***.

**On**: Enable the displacement.