.. _fwdModAmpData:

.. include:: <isonum.txt>

Forward model magnetic amplitude data in GIFtools
=================================================

In this recipe, we step through forward modelling magnetic amplitude data, starting from a TMI data file, a topography file, and a 3D mesh. At the bottom of this page, you will find the :ref:`files used in this recipe as well as the complete project and output files <AmpExample>`.

This recipe requires the following steps:

#. :ref:`Import the necessary files <ampStep1>`
#. :ref:`Invert for an equivalent source model <ampStep2>`
#. :ref:`Forward model amplitude data <ampStep3>`

.. _ampStep1:

**STEP 1: Import the necessary files**

Start GIFtools or open an already existing project. Because we will be loading in a few files, it is easiest to :ref:`set the working directory <utilSetWorkDir>` to the folder where the files are located and/or where you would like to do the forward model. 

The first step is then to import the magnetic data, the topography file, and the 3D mesh. :ref:`Importation of data <data>` can slightly differ, depending on the file type (GIF format, Geosoft XYZ, etc). For this example, the magnetic data and the topography file are both in GIF format. Both are imported using the following menus:

- For magnetic survey locations: **Import** |rarr| **Data** |rarr| **Magnetics** |rarr| GIF format
- For topography: **Import** |rarr| **Data** |rarr| **Topography** |rarr| 3D GIF (3D XYZ)
- For the 3D mesh: **Import** |rarr| **Mesh** |rarr| **3D**

.. figure:: ../../images/createOctreeMesh/importdata.png
        :figwidth: 75%
        :align: center

Once the data are loaded, GIFtools will have the three items shown in the project tree on the left. It's a good idea to regularly :ref:`save <projSave>` your project!

.. note:: If you have a susceptibility model, you can :ref:`import the model <importModel>` and skip directly to :ref:`forward modelling the amplitude data <ampStep3>`.

Before we can solve for an equivalent source model for this magnetic data, we need to :ref:`set the I/O for the data and uncertainties <setioHeaders>`. This means we need to :ref:`assign uncertainties to the data first <assignUncert>`.

Use the menu structure to set the uncertainty for the magnetic data:

**Data Manipulation** |rarr| **Assign uncertainties**

A dialog pops up to add a percentage and/or a floor to each header. We completed the dialog by clicking the **Assign** checkbox for the header "B" and using 0 for percentage and 0.5 nT for the floor. Click "OK" to apply the changes. Now use the menu structure to set the I/O headers for the data:

**Data Manipulation** |rarr| **Set I/O headers**

For this example, make sure the total-field anomaly is set the "B" and the uncertainty to "B_uncert" by choosing these from the drop-down boxes. Click "OK" to close the dialog and apply the changes. The info panel for the magnetic data item will have updated and all minimum data requirements for the inversion are now set (indicated using ** in the info panel).

.. _ampStep2:

**STEP 2: Invert for an equivalent source model**


.. _ampStep3:

**STEP 3: Forward model amplitude data**



.. _ampExample:

.. example:: The magnetics data file, topography file, and 3D mesh along with a GIFtools project to repeat the above steps to forward model amplitude data: `download <https://www.eoas.ubc.ca/~sdevries/GIFtoolsExamples/ForwardModelAmplitudeData_example.zip>`__


