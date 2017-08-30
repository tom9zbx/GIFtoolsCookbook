.. _createMagInv:

.. include:: <isonum.txt>

Create a magnetics inversion
============================

There are four different inversion objects that can be created to invert magnetic data using a 3D mesh. The first three are using the program ``MAG3D`` with version control (5.0, 5.1, 6.0). The fourth is a magnetic-vector inversion using the program ``MVI``. To use an octree mesh, the code ``OCTMAGDE`` can be used. The menus needed to create these are:

**Create** |rarr| **Inversion** |rarr| **Magnetics** |rarr| **Induced (MAG3D 5.0)**

**Create** |rarr| **Inversion** |rarr| **Magnetics** |rarr| **Induced (MAG3D 5.1)**

**Create** |rarr| **Inversion** |rarr| **Magnetics** |rarr| **Induced/amplitude (MAG3D 6.0)**

**Create** |rarr| **Inversion** |rarr| **Magnetics** |rarr| **MVI (magnetic vector)**

**Create** |rarr| **Inversion** |rarr| **Magnetics** |rarr| **PDE (octree)**

.. figure:: ../../../images/createInv.png
    :align: center
    :width: 400

**NOTE**: GIFtools inversion objects will take care of the prerequisite weighting and sensitivity programs prior to inversion for the user.


