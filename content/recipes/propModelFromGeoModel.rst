.. _propModelFromGeoModel:

.. include:: <isonum.txt>

Create a physical property model from a geologic model
======================================================

In GIFtools, a geologic model can be edited to generate a physical property model. This recipe goes through the steps to do so. To start, a GEOmodel is required. A geology model can be created in :ref:`Model Builder <createModelBuilder>` (e.g., :ref:`from an isosurface <IsoSurfaceToGeoModel>`).

The example being used throughout this recipe is based on a GEOmodel created from an isosurface of a susceptibility model. This particular geologic model contains three units: (0) air, (1) the background, and (2) the anomalies, as shown in the figure below.

.. figure:: ../../images/createModFromGeo/model.png
	:align: center
	:figwidth: 100%

Any geology model will have a geologic definition. To edit the definition, use the menu for the geology model: **Geology Model** |rarr| **Geology definition** |rarr| **Edit**. 

.. figure:: ../../images/createModFromGeo/editdef.png
	:align: center
	:figwidth: 100%

This brings up the following window:

.. figure:: ../../images/createModFromGeo/geodef.png
	:align: center
	:figwidth: 100%

Currently, there are no physical properties assigned to each of the units. The units have the header "Index" and in this example there are 3. Click on "Add column" to add a column for physical properties. A window will appear, prompting for the name of the new column:

.. figure:: ../../images/createModFromGeo/addcolumn.png
	:align: center
	:figwidth: 50%

Enter the desired name. For this example, the name used is "susValue". Click "Value" if the column will contain numbers (e.g., conductivity values) or "String" if the column will contain words (e.g., rock names). Here we are interested in physical property values so we click "Value". The window will close and the new column appears in the geology definition, as shown below:

.. figure:: ../../images/createModFromGeo/geodef2.png
	:align: center
	:figwidth: 100%