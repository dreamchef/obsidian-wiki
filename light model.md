
#graphics

describes the interaction between materials and light sources

$$A_I = \text{(ambient reflection)(ambient light intensity)}$$

$$D_I = \text{light intensity}( \text{diffuse reflection} * \text{(normal} \bullet \text{light direction))}$$

$$S_I = \text{light intensity}(\text{spec. reflection} * (\text{normal} \bullet \text{halfway vector})^{\text{spec. exp.}})$$
$$I = A_I + \Sigma (\text{light intensity})(D_I + S_I)$$

Sum refers to more than one possible source.

# Specific Models
- [[Phong shading]]
- [[Gourad shading]]
- [[Flat shading]]
- Cook-Torrence
- Ward