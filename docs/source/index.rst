Wind-AE: Documentation
===================================

**Wind-AE** (/windy/) is a predictive 1D, steady state, hydrodynamic Parker wind relaxation code for modeling photoevaporative atmospheric escape of exoplanets. The model builds upon `Murray-Clay et al. (2009)`_ and includes the ability to model metals in the wind and full XUV stellar spectra.

.. _Murray-Clay et al. (2009): https://ui.adsabs.harvard.edu/abs/2009ApJ...693...23M/abstract

.. note::
   This model is valid for upper atmospheres between P~10^{-4} bars and the Coriolis turning radius (computed self consistently in code, usually a few $R_P$).
   


**Wind-AE** is a python-wrapped ``C`` code based on `Numerical Recipes in C`_'s relaxation algorithm. It solves the finite difference versions of steady state ioinization balance, mass, momentum, and energy conservation equations for a hydrodynamic Parker wind. 
As a relaxation code, it runs quickly, but the relaxation method is sensitive to having a good initial guess for the solution in order to numerically converge to the final solution. With that in mind, we provide a number of starting points for simulations in the ``saves/`` folder and include a python wrapper which handles ramping from the initial guess solution to a final solution that is far from it in parameter space.

.. _Numerical Recipes in C: https://numerical.recipes/

Check out the :doc:`usage` section for further information, including
how to :ref:`installation` the project.





.. note::

   This project is under active development. Please report bugs and we appreciate your patience as we roll out changes.

Contents
--------

.. toctree::

   usage
   api
