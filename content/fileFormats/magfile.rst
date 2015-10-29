.. _magfile:

Magnetic observations: GIF file
-------------------------------

This file is used to specify the inducing field parameters, anomaly
type, observation locations, and the observed magnetic anomalies with
estimated standard deviation. The values of parameters specifying the
inducing field anomaly type and observation locations are identical to
those in file. The output of the forward modelling program has the same
structure except that the column of standard deviations for the error is
omitted. GIFtools will read either format through when importing a magnetic data set in GIF format. The structure of the GIF-formatted magnetics observations file is:

| \|ccccccc\|
| incl & decl & geomag & & & &
| ainc & adec & dir & & & &
| ndat & & & & & &
| E\ :math:`_1` & N\ :math:`_1` & ELEV\ :math:`_1` & [ainc\ :math:`_1` &
  adec\ :math:`_1`] & Mag\ :math:`_1` & Err\ :math:`_1`
| E\ :math:`_2` & N\ :math:`_2` & ELEV\ :math:`_2` & [ainc\ :math:`2` &
  adec\ :math:`_2`] & Mag\ :math:`_2` & Err\ :math:`_2`
| :math:`\vdots` & :math:`\vdots` & :math:`\vdots` & :math:`\vdots` & :math:`\vdots` & :math:`\vdots` &
| E\ :math:`_{ndat}` & N\ :math:`_{ndat}` & ELEV\ :math:`_{ndat}` &
  [ainc\ :math:`_{ndat}` & adec\ :math:`_{ndat}`] & Mag\ :math:`_{ndat}` &
  Err\ :math:`_{ndat}`

Parameter definitions:

-  Lines starting with ! are comments.

-  Inclination and declination of the inducing magnetic field. The
   declination is specified positive east with respect to the northing
   used in the mesh and locations files. The inclination is positive
   down.

-  Strength of the inducing field in nanoTesla (nT).

-  Inclination and declination of the anomaly projection. Set for a
   multi-component dataset and for a single component dataset where all
   the observations have the same inclination and declination of the
   anomaly projection.

-  Number of observations. When single component data are specified the
   number of observations is equal to the number of data locations. When
   multi-component data are specified the number of observations will
   exceed the number of data locations. For example, if three-component
   data are specified at :math:`N` locations, the number of observations
   is :math:`3N`.

-  Easting, northing, and elevation of the observation measured in
   meters. Elevation should be above the topography for surface data,
   and below the topography for borehole data. The observation locations
   can be listed in any order.

-  Inclination and declination of the anomaly projection for observation
   n. This is used only when . The brackets :math:`[\cdots]` indicate
   that these two field are optional depending on the value of .

-  Magnetic anomaly data, measured in nT.

-  Standard deviation of Mag\ :math:`_n`. This represents the absolute
   error. It CANNOT be zero or negative.

**NOTE:** It should be noted that the data are **extracted anomalies**
which are derived by removing the regional from the field measurements.
It is crucial that the data be prepared as such.

Examples 
^^^^^^^^

The following are two examples of data files. The first example file
specifies a set of total field anomaly data, and the second example file
provides a set of multi-component borehole data.

**Example 1**: single-component data

| \|cccccl\|
| 45.0 & 45.0 & 50000 &
| 45.0 & 45.0 & 1 &
| 144 &
| 0.00 & 0.00 & 1.00 & 0.174732E+02 & 0.598678E+01 &
| 0.00 & 50.00 & 1.00 & 0.265550E+02 & 0.613890E+01 &
| 0.00 & 100.00 & 1.00 & 0.311366E+02 & 0.629117E+01 &
| & & & & &
| 1000.00 & 900.00 & 1.00 & -0.109595E+01 & 0.530682E+01 &
| 1000.00 & 950.00 & 1.00 & -0.902209E+01 & 0.523738E+01 &
| 1000.00 & 1000.00 & 1.00 & -0.397501E+01 & 0.518496E+01 &

**Example 2**: Multi-component data

| \|cccccl\|
| 45.0 & 45.0 & 50000 &
| 45.0 & 45.0 & 0 &
| 144 &
| -12.50 & -137.50 & -12.50 & 0.0 & 0.0 &

+----------------+----------------+
| 0.134759E+03   | 0.200000E+01   |
+----------------+----------------+

| 
| -12.50 & -137.50 & -37.50 & 0.0 & 0.0 &

+----------------+----------------+
| 0.162606E+03   | 0.200000E+01   |
+----------------+----------------+

| 
| -12.50 & -137.50 & -62.50 & 0.0 & 0.0 &

+----------------+----------------+
| 0.165957E+03   | 0.200000E+01   |
+----------------+----------------+

| 
| & & & & &
| -12.50 & -137.50 & -37.50 & 90.0 & 0.0 &

+----------------+----------------+
| 0.662445E+02   | 0.200000E+01   |
+----------------+----------------+

| 
| -237.50 & -12.50 & -362.50 & 90.0 & 0.0 &

+----------------+----------------+
| 0.693134E+02   | 0.200000E+01   |
+----------------+----------------+

| 
| -237.50 & -12.50 & -387.50 & 90.0 & 0.0 &

+----------------+----------------+
| 0.608605E+02   | 0.200000E+01   |
+----------------+----------------+

| 

