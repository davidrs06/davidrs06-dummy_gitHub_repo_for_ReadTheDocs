Usage
=====

.. _installation:

Installation
------------

To use the fake_python_package, first install it using pip:

.. code-block:: console

   (.venv) $ pip install fake_python_package # <- to be tested after upload to pipy

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the :py:func:`fake_python_package.fake_python_module.get_random_ingredients` function:

.. autofunction:: fake_python_package.fake_python_module.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`fake_python_package.fake_python_module.get_random_ingredients`
will raise an exception.

.. autoexception:: fake_python_package.fake_python_module.InvalidKindError

For example:

>>> from fake_python_package import fake_python_module
>>> fake_python_module.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

