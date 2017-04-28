.. _IsoSurfaceToGeoModel:

.. include:: <isonum.txt>

Create a geologic model from an isosurface
==========================================

In GIFtools, a geologic model can be generated from any physical property model (e.g., a density contrast model or a conductivity model). This recipe outlines the steps to create a geologic model based on isosurfaces from a physical property model.

Open GIFtools and if desired, :ref:`set the working directory <projSetWorkDir>`.

In this recipe, the example uses a 3D mesh and a susceptibility model. :ref:`Import the 3D mesh <importMesh3D>` and then :ref:`import the corresponding model <importModel>`.

:ref:`View the model <viewModel>` and decide what the physical property values are for the isosurfaces(s). In this case, there is a single isosurface at 0.002 SI. This means this geologic model will have three units: 

#. Air (cells set to -100)
#. Background (cells with susceptibility between 0 and 0.002 SI)
#. Anomaly (cells with susceptibility 0.002 SI and up)

The figure below shows the example model used in this recipe.

.. figure:: ../../images/IsoToGEoMod/model.PNG
	:align: center
	:figwidth: 75%