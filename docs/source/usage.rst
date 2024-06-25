Usage
=====

.. _installation:

PICam Installation
------------
How to get vscode running on the camera computer:

- Open terminal

- Run commands as the root user:

.. code-block:: console
  
  sudo -s

- Navigate to the directory containing the cpp files: 

.. code-block:: console

    cd /opt/PrincetonInstruments/picam/samples/source code/platform independent

- Run the following command to open all .cpp files:

.. code-block:: console

    code --no-sandbox --user-data-dir=$HOME/.vscode-root ./*.cpp”

- Substitute the * to open a specific file

Compiling and running the code:
Navigate to the folder containing make files, and generate a new make file:
.. code-block:: console

    cd /opt/PrincetonInstruments/picam/samples/projects/gcc
    make -f [file].mk

If no errors, navigate to: ‘/opt/PrincetonInstruments/picam/samples/projects/gcc/objlin/x86_64/debug’
Run ‘./[file]’, and any additional arguments


To use Lumache, first install it using pip:


  pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

