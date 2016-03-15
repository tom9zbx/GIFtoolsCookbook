.. _generalFunctionality_index:

General functionality
=====================

All of the these functions can be accessed through the menus at the top after selecting the object in the GIFtools tree. The main categories presented here are:

- :ref:`project`
- :ref:`data`
- :ref:`mesh`
- :ref:`model`
- :ref:`fwd`
- :ref:`inv`
- :ref:`mb`
- :ref:`esrc`
- :ref:`util`


.. _project:

Project
-------

    .. toctree::
        :maxdepth: 1
    
        Load <project/load>
        Load a recent project <project/loadRecent>
        Add an existing project <project/addProject>        
        Save <project/save>
        Set the working directory <project/setWorkDir>
        Set the starting directory <project/setStartingDir>
        Set the number of OpenMP threads <project/setOMPthreads>        
        Find the version number <project/about>


.. _data:

Data
----

    **General functionality:**

    .. toctree::
        :maxdepth: 1

        data/editDataHeaders
        Delete columns <data/deleteDataColumns>
        Create topography <data/dataCreateTopo>
        Create 3D mesh <data/dataCreateMesh>
        Downsample <data/downsample>        
        Set input/output (i/o) headers <data/setioHeaders>
        Assign uncertainties <data/assignUncertainties>
        Perform a simple mathematical operation <data/constantCalculator>
        Perform column-to-column mathematical operation <data/columnCalculator>
        Add Gaussian noise <data/addNoise>
        Combine like objects <data/combineData>
        Delete data outside of a mesh <data/meshBasedRemoval>
        Calculate a polynomal trend <data/polyTrend>
        View in 3D, table format, or view statistics <data/viewData>
        Export <data/export>


    **Magnetics:**

    .. toctree::
        :maxdepth: 1

        Assign / Edit inducing field <data/editFieldParams>
        Remove IGRF <data/removeIGRF>


    **DC/IP:**
    
    .. toctree::
        :maxdepth: 1

        Add topography to locations <data/applyTopo>
        Apparent resitivity to/from normalized voltage <data/dcipGeoFactor>
        Project DC/IP 3D data onto a 2D lines for DCIP2D inversion <data/dcip3Dto2D>

    **EM:**

    .. toctree::
        :maxdepth: 1

        Extract time / frequency data <data/emTimeExtract>
        View / edit times or frequencies <data/emViewTime>

.. _mesh:

Mesh
----

    .. toctree::
        :maxdepth: 1

        mesh/createConstantModel
        mesh/createActiveCellsModel
        mesh/refineOctree
        View in 3D <mesh/viewMesh>        
        Export <mesh/export>

.. _model:

Model
-----

    .. toctree::
        :maxdepth: 1

        mesh/createConstantModel
        model/createActiveCells
        Set unit name <model/setUnit>
        Perform a simple mathematical operation <model/modelCalculator>
        Add polyhedra from property data <model/addPolyBlock>
        Assign values to air cells <model/assignAirValues>        
        View in 3D, table format, or view statistics <model/viewModel>
        Export <model/export>


.. _fwd:

Forward modelling
-----------------

    **Creating a object:**
   
    .. toctree::
        :maxdepth: 1

        Gravity <forward/grav3d>
        Magnetics <forward/mag3d>
        DC/IP <forward/dcipFwd>

    **General functionality:**

    .. toctree::
       :maxdepth: 1

       Set the working directory <forward/setWorkDir>
       Edit options <forward/editOptions>
       Write files <forward/writeAll>
       Run <forward/run>
       Load results <forward/loadResults>
       Copy the item <forward/copyOptions>

.. _inv:

Inversion
---------

    **Creating an object:**

    .. toctree::
        :maxdepth: 1
        
        Through a workflow <inversion/inversionWorkflow>
        Gravity <inversion/grav3d>
        Magnetics <inversion/mag3d>
        DC/IP <inversion/dcipInv>        
        ZTEM or MT <inversion/mtz3d>
        FEM <inversion/femInv>

    **General functionality:**

    .. toctree::
       :maxdepth: 1

       Set the working directory <inversion/setWorkDir>
       Edit options <inversion/editOptions>
       Write files <inversion/writeAll>
       Run <inversion/run>
       Load results <inversion/loadResults>
       View results <inversion/viewInversion>
       Copy the item <inversion/copyOptions>


.. _mb:

ModelBuilder module
-------------------

 .. toctree::
        :maxdepth: 1

        Create modelBuilder <modelBuilder/createModelBuilder>


       
.. _esrc:

Equivalent-source processing
----------------------------

    **Creating an object:**

    .. toctree::
        :maxdepth: 1

        Gravity <esProcessing/grav3d>
        Magnetics <esProcessing/mag3d>

    **General functionality:**

    .. toctree::
       :maxdepth: 1

       Set the working directory <esProcessing/setWorkDir>
       Edit options <esProcessing/editOptions>
       Write files <esProcessing/writeAll>
       Run <esProcessing/run>
       Load results <esProcessing/loadResults>
       View results <esProcessing/viewInversion>
       Copy the item <esProcessing/copyOptions>

.. _util:

Fortran utility programs
------------------------

    **Creating an object:**

    .. toctree::
        :maxdepth: 1

        OcTree mesh for E3D <utilityCodes/e3doctreeMesh>
        OcTree mesh for OCTMAGDE <utilityCodes/magoctreeMesh>
        Interpolate a 3D model onto another mesh <utilityCodes/interpolateModel>        

    **General functionality:**

    .. toctree::
       :maxdepth: 1

       Set the working directory <utilityCodes/setWorkDir>
       Edit options <utilityCodes/editOptions>
       Run <utilityCodes/run>
       Load results <utilityCodes/loadResults>


