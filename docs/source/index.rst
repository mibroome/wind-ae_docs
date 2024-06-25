Wind-AE: Documentation
===================================

**Wind-AE** (/windy/) is a predictive 1D, steady state, hydrodynamic Parker wind relaxation code for modeling photoevaporative atmospheric escape from exoplanets.

A `C` code based on *Numerical Recipes in C*'s relaxation algorithm solves the finite difference versions of steady state ioinization balance, mass, momentum, and energy conservation equations for a hydrodynamic Parker wind. As a relaxation code, it runs quickly, but the relaxation method is sensitive to having a good initial guess for the solution, so we provide a number of starting points for simulations in the `saves/` folder and include a python wrapper handles ramping from the initial guess solution to a final solution that is far from it in parameter space.

Check out the :doc:`usage` section for further information, including
how to :ref:`installation` the project.


It pulls data from the `Open Food Facts database <https://world.openfoodfacts.org/>`_
and offers a *simple* and *intuitive* API.


.. note::

   This project is under active development. Please report bugs and we appreciate your patience as we roll out changes.

Contents
--------

.. toctree::

   usage
   api
