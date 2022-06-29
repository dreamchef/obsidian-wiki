---
id: cgu1s2v4uehpkr1qy7sz3ps
title: Lighting Calculation
desc: ''
updated: 1656468975960
created: 1654530813201
---
#graphics #method

Consider the RGB color model.  In order to calculate the amount of red $r$ in a vertex color, we must sum the red contributions $I_{i,r}$ from each individual light $L_i$ in the scene:
$$r = I_{0,r} +  I_{1,r} + ...$$

To calculate the contributions $I_{i,c}$, ...

$contribution =  ambient + angle(specular + diffuse)$
