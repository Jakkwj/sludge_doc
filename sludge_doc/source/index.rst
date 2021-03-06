===========
Sludge
===========



.. toctree::
    :hidden:
    :caption: This is a caption
    :titlesonly:

    模块/index


.. toctree::
    :hidden:
    :caption: about

    about
    ChangeLog/index


Welcome to Sludge's documentation.

Introduction
==============


Sludge is a **SaaS platform** for calculating the matrix like biochemical models (such as activated sludge models 1, 2 and 3). The aim of this project is to help people to build and calculate their own wasterwater treatment process easily.
The input of the whole process are only 3 excel xlsx files. By this way, you can check and make your own biological model conveniently.


The key features are:

- **Simple**:

  + only 3 excel files and you are good to go
- **Sharable**
- **Trackable**



This is a demo site for |theme_display|, generated as part of
`Sphinx Themes Gallery <https://sphinx-themes.org>`_.


Time Unit
==============
To unify the time unit in Sludge calcualtion, all time units will translated to ``'second'``.
There are 2 time units we should notice: **Parameter** and **Measured**.

Parameter
--------------
NOTE that Parameter time unit is fixed to be ``'day'`` and unchangable.
The Unit column in Parameter sheet of **BioModel.xlsx** is actually an annotation, it won't affect any calculation result.

For instant, if you set ``b_OHO_end`` (the endogenous respiration rate coefficient of ordinary heterotrophic organisms) to be 0.008 h :sup:`-1`, it will be recognized as 0.008 d :sup:`-1` rather than 0.2 d :sup:`-1` as you might expect.
So even for interpreted purpose, you should always set the time unit to be ``'day'`` in Unit column.


Measured
--------------
Measured time unit is setted in the TimeUnit column (only 1st row) in Tank sheet of **DataSet.xlsx**, which could only be: ``'second'``, ``'minute'``, ``'hour'`` or ``'day'``.
The Component (Measured sheet) and Flow (Link sheet) data will follow this time unit.













Snapshot
===========
.. image:: _static/images/Fig5__Sim_Targets__.png
.. image:: _static/images/Project__Eva_UncertaintyPCDF__(59).png


.. important::

    Let's Build Models Together.



.. important::

    This sample documentation was generated on |today|, and is rebuilt weekly.



