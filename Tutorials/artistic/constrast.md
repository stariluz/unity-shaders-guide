
# Contrast
Adjust the contrast of the input *In* by the amount of the input *Contrast*. If the value of contrast is 1, it returns *In*, if it's 0, returns the midpoint of *In*.

### Input.
In: Vector3
Contrast: Vector1

### Outputs.
Out: Vector3

## Controllers
This component has not controllers.

## Explanation
This is a code example (that the documentation gave us) this node can generate. I'm adding a little explanation.
```cs
 void Unity_Contrast_float(float3 In, float Contrast, out float3 Out)
{
    float midpoint = pow(0.5, 2.2);
    Out = (In - midpoint) * Contrast + midpoint;
}
```
