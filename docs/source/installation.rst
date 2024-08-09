Installation
============

``Wind-AE`` package requirements: ``numpy``, ``scipy``, ``matplotlib``,
``pandas``, ``cycler``.


Compile from source (development version)
---------------------------------------------------

First, clone the repository and navigate to it:

.. code-block:: bash

   git clone https://github.com/mibroome/wind_ae.git && cd wind_ae

And then compile ``p-winds`` from source:

.. code-block:: bash

   python -m pip install -e .

Make the ``C`` code:

.. code-block:: bash

   make
