.. _importActiveModel:

.. include:: <isonum.txt>

Importing an active-cell model
==============================

Importing a model first requires a mesh. The import dialog will prompt the user to either choose an existing mesh in the project or browse to load another. **Active cells will contain only values of -1, 0, or 1.**

Use the main project menu: **Import** |rarr| **Model** |rarr| **Active**

.. figure:: ..\..\..\images\importModel.png
    :align: center
    :width: 400


Prerequisites
-------------
Import a mesh:

.. toctree::
   :maxdepth: 1

   2D mesh <../mesh/importMesh2D>
   3D mesh <../mesh/importMesh3D>    
   OcTree mesh <../mesh/importMeshOctree>


File formats
------------

Active models can only be imported via :ref:`GIF-formatted <modelfile>` files





