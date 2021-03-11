### Discontinuities

- Moho 
- Core mantle boundary 

- Hales (75-130km)

- Lehmann (220km)

- 510km discontinuity

__Primary discontinuities__ are those that can be observed everywhere. Moho and CMB are primary. 

__Secondary discontinuities__ are those that are not necessarily observed everywhere. Hales, Lehmann and the 510km discontinuity are examples. 

__Lithosphere__ is the crust and the uppermost mantle. It includes the MOHO. 

__Lithosphere-Asthenosphere boundary__: also known as _LAB_. The velocities increase at discontinuities. In this case there is a velocity decrease. 

At the moho, there is an increase in velocity. 

### Earthquakes

The **focus** is present in the subsurface.

**Epicenter** is present on the surface.

The angle subtended at the centre of the earth between the epicenter and the observation station is denoted by $\Delta$. 

The __back azimuth__ is the angle between the north and the location of the earthquake as measured from the station, in the clockwise direction. 

The **_epicentral distance_** is calculated using, 
$$
ED=R\cdot \Delta
=6371\cdot\Delta
$$
For 1^o^, this corresponds to a distance of $111.2\text{km}$. 
$$
P=u\cdot\sin\theta
$$
where, $u=\frac{1}{v}$. 
$$
T=2\sum_{i=1}\frac{u_i^2\Delta ^2_i}{\sqrt{u_i^2-p^2}}
$$
where, $u_i>p$. 

We only calculate the time upto the __turning point.__, which is half the total distance. 

The projection of a point at a depth on the surface is called the  __piercing point__.

If we consider an infinite number of layers, we get,
$$
T=2\int_0^{z_p}\frac{u^2(z)dz}{\sqrt{u^2(z)-p^2}}
$$
The distance will be given by, 
$$
X=2\int_0^{z_p}\frac{p(z)dz}{\sqrt{u^2(z)-p^2}}
$$
All the calculations are made from surface to surface. If however we are only required to calculate between some given distance, we should use the integral between the range, without the factor of two. 

If $X$ increase results in a decrease in $p$, we call it a __Prograde__ graph. In other words,
$$
\frac{dx}{dp}<0
$$
The ray parameter is calculated by, 
$$
\frac{dT}{dx}
$$
If we encounter a discontinuity (with a large *increase* in velocity), we observe a decrease in $X$. In this case we call it a __retrograde__ graph. It is characterised by,
$$
\frac{dX}{dp}>0
$$

> HW1: What happens in the case of a low velocity zone?

Question: find X and T for three layers with velocities $4,5,6$ and depth $5km$ each, with $p=0.15$. 

Since $p<u_i$, (note that $u=\frac{1}{v}$) we have,
$$
x=\ 2\cdot p\cdot5\cdot\left(\frac{1}{\sqrt{\left(\frac{1}{4}\right)^{2}-p^{2}}}+\frac{1}{\sqrt{\left(\frac{1}{5}\right)^{2}-p^{2}}}+\frac{1}{\sqrt{\left(\frac{1}{6}\right)^{2}-p^{2}}}\right)\\=39.4
$$
If however, $p>u_i$, we simply remove the terms corresponding to $i$. This happens because the wave undergoes reflection at that layer.



