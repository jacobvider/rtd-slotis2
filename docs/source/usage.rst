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

- Open all .cpp files, substituting the * with the file name for a specific file

.. code-block:: console

    code --no-sandbox --user-data-dir=$HOME/.vscode-root ./*.cpp”

Compiling and running the code:
Navigate to the folder containing make files, and generate a new make file:

.. code-block:: console

    cd /opt/PrincetonInstruments/picam/samples/projects/gcc

    make -f [file].mk

    cd /opt/PrincetonInstruments/picam/samples/projects/gcc/objlin/x86_64/debug

To run the executable: 

.. code-block:: console

  ./[file] [arguments]
