.. _setOMPthreads:

.. include:: <isonum.txt>

Set the number of threads to run an inversion
=============================================

GIF inversion programs use OpenMP to parallelize matrix-vector multiplicatoin and sensitivity calculations in linear inversions. GIFtools allows the user to change the number of OpenMP threads so the inversions do not slow down the CPU. Use the menu structure:

**Project** |rarr| **Set properties** |rarr| **Set openMP threads for Fortran codes**

.. figure:: ../../../images/projectPropMenu.png
    :align: center
    :width: 400

**NOTE 1:** The shortcut for the functionality is ``control + shift + d``.


**NOTE 2:** GIFtools will only find out the number of *cores* the CPU is operating on and not the actual threads. If you would like to manage the number of threads the inversions use, the environment variable ``OMP_NUM_THREADS`` will need to be set (see below).


Setting environment variable for OpenMP threads (optional)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To set the maximum number of OpenMP threads, an environment variable will need to be established. Follow these steps:

1. Click on the windows menu and then *right-click* on **Computer** and click on **Properties**

.. figure:: ../../../images/openmpThreads1.png
   :align: center
 

2. Click on **Advanced System Settings** to get the the window below.

.. figure:: ../../../images/openmpThreads2.png
   :align: center


3. Click on **Environment variables** and then create a new variable (or edit if the variable ``OMP_NUM_THREADS`` exists) by clicking **new**:

.. figure:: ../../../images/openmpThreads3.png
   :align: center



4. Click **OK** then **Apply** and exit. Re-start GIFtools and the number of threads will appear.


**NOTE:** If you are unsure how many threads the computer has there are two ways of finding out:

#. Run a GIF program such as PFWEIGHT or MAGINV3D. The program will tell you how many threads it uses without by just bringing up a command prompt (``shift + right-click + open command window here``). The program will have to be pathed or perform this task in the parental directory of GIFtools.

#. Open Windows task manager (``right-click`` on bottom task bar then ``Start task manager``) and go to **Performance**. Count the number of windows in CPU Usage History (below is an example of 12):

.. figure:: ../../../images/openmpThreads4.png
   :align: center
   :width: 400


