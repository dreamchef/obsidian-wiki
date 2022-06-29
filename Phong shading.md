
#graphics 

Calculate shade at each vertex and interpolate normal, then interpolate shade.  

This method eliminates the mach bands in [[Gourad shading]].
# Reflection components
$$I = A_I + D_I + S_I$$
## Ambient
$A_R$ ambient reflection (vertex property)
$A_L$ ambient light intensity (light property)
$$A_I = A_R  A_L$$
## Diffuse
$L_I$ light intensity
$D_R$ diffuse reflection (vertex property)
$N$ vertex normal
$L_D$ incoming light direction (unit vector) ( #q does sign matter?)
$$D_I = L_I(D_R(N \bullet L_D))$$
## Specular
$L_I$ light intensity
$S_R$ specular reflection ( vertex property)
$S_E$ specular exponent (rough/shiny)
$N$ vertex normal
$H$ halfway vector between incoming light ray and direction of camera
$$S_I = L_I(S_R(N \bullet H)^{S_E})=$$
### Calculating $H$
$V$ viewing angle
$$H = \frac{L_D + V}{2}$$

Note that if a dot product is negative, set the associated intensity to zero ($\theta > 90^{\circ}$)
