.. _generalFunctionality_index:

General functionality
=====================

All of the these functions can be accessed through the menus at the top after selecting the object in the GIFtools tree.


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
        Add Gassian noise <data/addNoise>
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


    **EM:**

    .. toctree::
        :maxdepth: 1

        Extract time / frequency data <data/emTimeExtract>
        View / edit times or frequencies <data/emViewTime>


Mesh
----

    .. toctree::
        :maxdepth: 1

        mesh/createConstantModel
        mesh/createActiveCellsModel
        mesh/refineOctree
        View in 3D <mesh/viewMesh>        
        Export <mesh/export>

Model
-----

    .. toctree::
        :maxdepth: 1

        mesh/createConstantModel
        Set unit name <model/setUnit>
        Perform a simple mathematical operation <model/modelCalculator>
        Add polyhedra from property data <model/addPolyBlock>
        Assign values to air cells <model/assignAirValues>        
        View in 3D, table format, or view statistics <model/viewModel>
        Export <model/export>


Forward modelling
-----------------

    **Creating a object:**
   
    .. toctree::
        :maxdepth: 1

        Gravity <forward/grav3d>
        Magnetics <forward/mag3d>
        DC/IP <forward/dcipFwd>


Inversion
---------

    **Creating an object:**

    .. toctree::
        :maxdepth: 1

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


