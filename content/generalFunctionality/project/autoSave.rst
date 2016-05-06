.. _projAutoSave:

.. include:: <isonum.txt>

Project auto-save functionality
===============================

GIFtools will auto-save a *copy* of the project. The feature is helpful in case something was deleted, for some reason the program crashed, or you forgot to save the project before quitting GIFtools. The auto-save copy is called "GIFtoolsAutoSave.mat" and is located in the ``\Windows\Users\yourUserName`` (i.e., home) folder. Please note that the **current project file is not touched** when auto saving and that the auto-save project will be *over-written* each time this function is called. The project can be saved in its normal location by using the :ref:`Save project <projSave>` feature. The user may select the amount of passing time (in minutes) between auto saves. To set this time, use the menu structure below:

- **Project** |rarr| **Set properties** |rarr| **Set time between auto save**

.. figure:: ../../../images/projectPropMenu.png
    :align: center
    :width: 400

**NOTE 1:** The shortcut for saving a project is ``control + shift + t``.

**NOTE 2:** The counter for auto save automatically re-sets after a project has been saved. The user can see the last time an auto save occurred in the information panel by clicking on the project in the tree.

