

To a first approximation, the magnetic field of the Earth is a dipole field. At the earth's surface, the magnitude of the non dipole field is small. Today, the earth's best fitting dipole axis is aligned at 11.5^o^ with the earth's spin axis. 

This intersection of the best fitting dipole axis is called the _geomagnetic poles_ and similarly, the geomagnetic equator is defined. 

The two points on the surface of the earth where there is no horizontal component of magnetic field is termed the _magnetic poles_. In fact, these are __not__ the same as the geomagnetic poles. This is due to the deviation from a dipolar magnetic field. Similarly, the magnetic equator is defined.

#### Variations

Short term variation is majorly caused by the sun, due to the solar wind.

Long term variation is used to date the oceanic lithosphere.

In the intermediate term, the pole wanders by a few degrees a century and is called _secular variation_. On geologic time scales, on average, the geomagnetic field axis has been aligned with the earth's spin axis. Hence, we approximate the dipole field as aligned with the earth's spin axis, as this is critical for all paleomagnetic work.

### Magnetic potential

$$
V(\mathbf{r})=\frac{1}{4\pi r ^3}\cdot\mathbf{m}\cdot\mathbf{r}
$$

Where $m$ is the dipole moment which in the case of Earth has a magnitude of $7.94\cdot10^22Am^{-2}$.  The field at any position is given by,
$$
B(\mathbf{r}) = -\mu_0\nabla V(\mathbf{r})
$$
Where, $\mu_0=4\cdot\pi\cdot10^{-7}kgmA^{-2}s^{-2}$. We can expand $B(\mathbf{r})$ as 
$$
B(\mathbf{r})=(B_r,B_\theta,B_\phi)
$$
We can calculate the components using the previous equation. We get,
$$
B_r=-\frac{2\mu_0 m \cos \theta}{4\pi r^3}\\\\
B_\theta=-\frac{\mu_0 m \sin\theta}{4\pi r^3}\\\\B_\phi=0
$$
That $B_\phi$ should be 0 is obvious by symmetry. The magnitude of the magnetic field at any point is given by,
$$
B=\frac{\mu_0m}{4\pi r^2}\sqrt{1+3\cdot\cos^2\theta}
$$
Define,
$$
B_0:=\frac{\mu_0m}{4\pi R^2}
$$
then, on the earth's surface,
$$
B_r(R,\theta,\phi)=-2B_0\cos\theta\\
B_\theta(R,\theta,\phi)=-B_0\sin \theta
$$
The inward radial component ($-B_r$) is called $Z$.

### Inclination

The angle between the horizontal $H$ and the (negative) vertical component $Z$ is called inclination $I$. It is given by,
$$
\tan I = \frac{Z}{H}\\=2\cdot\frac{\cos\theta}{\sin \theta}\\=2\cot \theta\\\tan I=2\tan \lambda
$$
Where, $\lambda = 90-\theta$, also called the latitude. 

### Declination

Defined as the azimuth of the horizontal component of magnetic field. Measured in degrees East or West of north. 

## Magnetisation

As volcanic rocks cool, they pass through critical temperatures at which the iron minerals acquire spontaneous magnetisation. Once they are lower than the _blocking temperature_, the magnetised grains cannot be reorientied. Thus the rocks have a magnetic moments aligned in the direction of the earth's magnetic field, at the time of cooling. This magnetisation is called _thermoremanent magnetisation_. 

Sedimentary rocks acquire magnetisation through 2 ways:

1. Detrital remanent magnetisation: Occurs during the deposition of sedimentray rocks. If deposited in water, previously magnetised small grains align with their magnetic moments parallel to the earth's magnetic field as they fall.
2. Chemical remanent magnetisation: Occurs after deposition during the chemical growth of iron oxide grains. Chemical remanent magnetisation is however, a secondary magnetisation. 

#### Susceptibility

Induced magnetisation $\mathbf{M}$ is the magnetisation induced when the rock is put into the earth's magnetic field $\mathbf{B}$. It is given by,
$$
\mu_0\mathbf{M}(\mathbf{r})=\chi\mathbf{B}(\mathbf{r})
$$
Where, $\chi$ is the magnetic susceptibility. For basalts it varies from $10^{-4}$ to $10^{-1}$ and hence is much weaker than the earth's magnetic field. 

### Konigsberger ratio $Q$

Defined as the ratio of remanent magnetisation to induced magnetisation. Measurement of the angle of inclination of the remanent magnetisation gives the magnetic paleolatitude for that continent. However, if the continent has moved, or if the rock was tilted, the magnetic latitude so determined will be different from from its present latitude. This gives us a method of determining past _latitudes_ of continents. 