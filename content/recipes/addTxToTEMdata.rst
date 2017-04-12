.. _addTxToTEMdata:

.. include:: <isonum.txt>

Add transmitter information to a TEM data object
================================================

.. warning:: This page is under construction!

After a :ref:`time-domain EM data from a csv or xyz file <importVTEMdata>` has been imported into GIFtools, the transmitter information is still missing in the TEMdata object. This recipe steps through adding in the transmitter information in three different ways:

#. Loading a file

#. Creating airborne EM (AEM) coincident loop sources

#. Creating AEM offset loop sources

To add transmitters to a TEM data object, use the menus: **TEM data** |rarr| **Add transmitters** and select the desired method.

.. figure:: ../../images/addTxtoTEMdata/menu.PNG
        :align: center
        :figwidth: 75%

Loading a transmitter file
--------------------------

The transmitter file uses a "block" format. The types of EM transmitters available are:

- Large-loop,

- Line-current,

- Dipole, and

- Loop

Refer to the :ref:`EM transmitter formats page <emTransmitters>` for detailed information. Each transmitter will have its own "block" in the transmitters file.

Creating AEM coincident loop sources
------------------------------------

Creating AEM offset loop sources
--------------------------------

Additional notes and tips
-------------------------

**Note**: When creating AEM offset loop sources, double check that the location of the source is correct. You can do this by viewing the sources and receivers in the VTK viewer. Click **Sources** in the control panel to view the source locations.

**Tip**: If you have a large data set loaded into GIFtools and plan to downsample the data before inversion, it is recommended to **first** downsample and **then** assign transmitters to safe computation costs.
