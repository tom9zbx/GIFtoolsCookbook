.. _videoTutorials:

Video Tutorials
===============

Below is our entire collection of video tutorials!

- :ref:`Overview and general functionality <VToverview>`

**Data types**

- :ref:`Magnetics data <VTmagdata>`
- :ref:`Gravity data <VTgravdata>`
- :ref:`DC data <VTdcdata>`
- :ref:`IP data <VTipdata>`
- :ref:`Frequency-domain EM data <VTfemdata>`
- :ref:`Time-domain EM data <VTtemdata>`
- :ref:`Magnetotellurics data <VTmtdata>`
- :ref:`Z-axis tipper data <VTztemdata>`
- :ref:`Physical property and borehole data <VTppdata>`
- :ref:`Topography data <VTtopodata>`

**Meshes**

- :ref:`2D tensor mesh <VT2dmesh>`
- :ref:`3D tensor mesh <VT3dmesh>`
- :ref:`OcTree mesh <VTocmesh>`

**Models**

- :ref:`Cell-centred discretized model <VTccmodel>`
- :ref:`Face-centred discretized model <VTfcmodel>`

.. _VToverview:

Overview and general functionality covering all data types
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- Main look and feel of GIFtools: `tutorial <https://www.youtube.com/embed/Kqm0TyNJ-vQ>`_ 
- Import ascii-based XYZ files: tutorial
- Import ascii-based CSV files: tutorial
- Import ascii-based XYZ or CSV files for EM data: tutorial
- Import GIF-formatted files: tutorial
- Change the number of openMP threads for executables and find the version number: tutorial
- General data GUI: tutorial
- General model GUI: tutorial
- Create a tensor mesh: tutorial
- Using the modelBuilder module: tutorial
- Assign uncertainties to any data set: tutorial
- Use of data calculators: tutorial
- Use of calculator for models: tutorial

Data types
^^^^^^^^^^

.. _VTmagdata:

**Magnetics data (MAGdata)**

- I/O of GIF-formatted mag3d data files: see :ref:`general <VToverview>` functionality
- I/O of ascii-based CSV and XYZ file type: see :ref:`general <VToverview>` functionality
- Change/set (anomaly) inclinations, declinations, and field strength: tutorial
- Remove DC bias: tutorial
- De-trend data with polynomial fits: tutorial (or via the data GUI)
- Assign standard deviations (% and/or floor) to data: see :ref:`general <VToverview>` functionality
- Edit datum or standard deviation or completely remove them: see :ref:`general <VToverview>` functionality
- Output files for forward modelling: tutorial
- Set up input files for use with mag3d inversion: tutorial
- Read output files from mag3d and view predicted data, recovered models, and inversion diagnostics (e.g., Tikhonov curve): tutorial
- Perform joint inversion on multiple magnetic data sets with mag3d: tutorial
- Peform equivalent source processing (with magsenes and maginves): tutorial

.. _VTgravdata:

**Gravity data (GRAVdata)**

- I/O of GIF-formatted grav3d data files: see :ref:`general <VToverview>` functionality
- I/O of ascii-based CSV and XYZ file type: see :ref:`general <VToverview>` functionality
- De-trend data with polynomial fits: see :ref:`magnetic data <VTMagdata>` or via the data GUI
- Assign standard deviations (% and floor) to data: see :ref:`general <VToverview>` functionality
- Edit datum or standard deviation or completely remove them: see :ref:`general <VToverview>` functionality
- Output files for forward modelling
- Set up input file and output files for use with grav3d inversion
- Read output files from grav3d and view predicted data, recovered models, and inversion diagnostics

.. _VTdcdata:

**Direct current data (DCdata)**

.. _VTipdata:

**Induced polarization data (IPdata)**

.. _VTfemdata:

**General frequency-domain EM data (FEMdata)**

.. _VTtemdata:

**General time-domain EM data (TEMdata)**

.. _VTmtdata:

**Magnetotelluric EM data (MTdata)**

.. _VTztemdata:

**Z-Axis tipper EM data (ZTEMdata)**

.. _VTppdata:

**Physical property data (BOREdata and PROPdata) via modelBuilder**

.. _VTtopodata:

**Topography data (TOPOdata)**

Meshes
^^^^^^
In this section, we summarize the general functionality associated with each type of mesh that can be used within GIFtools.

.. _VT2dmesh:

**Two-dimensional tensor mesh (mesh2D)**

- I/O 2d meshes (for use with 2D codes)
- Keep track of topography and global coordinates of mesh

.. _VT3dmesh:

**Three-dimensional tensor mesh (mesh3D)**

- I/O and view 3D tensor meshes (for use with 3D codes)
- Create meshes internatlly with GIFtools for potential-field data: see :ref:`general <VToverview>` functionality
- Create ocTree meshes from tensor meshes (and interpolate the model)

.. _VTocmesh:

**OcTree meshes (meshOctree)**

- I/O and view the ocTree meshes (for use with ocTree codes)
- Fine-tune ocTree meshes by choosing which cells to coarsen and refine
- Easily create input files and (load) meshes interacting with Fortran-based executables (e.g., create_octree_mesh_e3d)

Models
^^^^^^
In this section, we summarize the general functionality associated with each type of model that can be used within GIFtools.

.. _VTccmodel:

**Cell-centred discretized models (GIFmodel)**

- I/O and view GIF models: see :ref:`general <VToverview>` functionality
- Re-mesh and transfer models from 3D to ocTree and vice versa
- Interpolate 2D models onto 3D models to combine information from multiple 2D inversions or cross sections
- Build reference models for inversion using other GIFmodels, geologic information, and/or borehole data: see :ref:`modelBuilder <VTppdata>` functionality
- Add convex-hull polygons/polyhedra or simple blocks to models for fast hypothesis testing
- Work with geology models that are accompanied with a definition to define property values, upper and lower bounds, rock type, and/or notes
- Edit models via the painting tool
- Use a simple calculator to convert between units and change the unit description: see :ref:`general <VToverview>` functionality
- Create active cell models from topography data (TOPOdata)
- Create active cell models from locations to choose where cells should be inactive
- Create simple constant-valuye models:
- Format allows for multiple models to be exported into bound file(s) for inversion (through GIFinversion objects)

.. _VTfcmodel:

**Face discretized models (FACEmodel)**

- I/O and view GIF models discretized on faces (e.g., weighting files): see :ref:`general <VToverview>` functionality (model GUI will view FACEmodels)
- Create face weighting for inversion based on a reference model: see :ref:`modelBuilder <VTppdata>` functionality
- Edit weighting parameters with ease with our painting tool
- Easily create input files and (load) face models interacting with Fortran-based executables (e.g., create_interface_weights)

