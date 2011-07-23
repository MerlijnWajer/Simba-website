.. Simba documentation master file, created by
   sphinx-quickstart on Sat Jul 23 12:29:37 2011.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to the home of Simba!
=============================

Welcome to the website of the Simba project.

If you're new to Simba, you'll want to read :ref:`whatis`.
To download Simba and view screenshots see :ref:`download` and
:ref:`screenshots`.

.. forums, contact, bugs, documentation, source

*Contents:*

    -   :ref:`whatis`
    -   :ref:`download`
    -   :ref:`documentation-ref`
    -   :ref:`download`
    -   :ref:`bugs`
    -   :ref:`tools`
    -   :ref:`screenshots`

.. _whatis:

What Is Simba?
==============

Simba is a program used to repeat certain (complicated) tasks. Typically these
tasks involve using the mouse and keyboard. Simba is programmable, which means
you can design your own logic and steps that Simba will follow, based upon
certain input.

This "input" can vary greatly; from data in files to colors and text on the screen.

Simba is:
    *   Open Source. (under the GPL license) (For more information see
        :ref:`source`.
    *   Free.
    *   Reliable but still maturing.
    *   Cross platform.

Simba can:
    *   Find and read colours on the screen.
    *   Click or move the mouse to a specific position on the screen. Typically
        this is the position of a found color or bitmap.
    *   Read text on the screen and turn it into actual text. (Optical Character
        Recognition)
    *   Capture and analyse images on the screen.
    *   Read and write files.
    *   Connect to the internet to read websites and post data to them.
    *   Run pascal programs for you. If you're a bit creative you can have a lot
        of fun stuff with Simba, you could even make a game in it!

and more. Start now by :ref:`download`.

Currently Simba is still in its beta stages; this includes the documentation_.
You will probably notice some parts of the documentation aren't finished or are just
plain missing. Don't be fooled by the look of the documentation as it is
identical to this homepage, in the future they may be merged.

.. _documentation: http://docs.villavu.com/simba/
.. _download:

Downloading Simba
=================

Simba runs on a few platforms, but currently only runs well on Windows.

Windows
-------

Simba for Windows can be downloaded as installer_, a portable build will follow
later. It will associate *.simba* files with Simba.


.. _installer: http://simba.villavu.com/bin/Release/Current/SimbaInstaller.exe

Installation Notes
~~~~~~~~~~~~~~~~~~


-   If you run Windows Vista or Windows 7, then you have to options; install Simba
    to *Program Files* and run it as administrator, or install it to a place that
    does not require ``Administrator`` permissions to write to - such as *My
    Documents* or just in a folder on your *Desktop*.

-   If you want to use SRL, see this `guide <http://docs.villavu.com/simba/gettingstarted.html#setting-up-srl-4-with-simba>`_.

-   For the script manager, see this `article <http://docs.villavu.com/simba/features/scriptmanager.html>`_ on the documentation_.


Linux
-----

Simba for Linux is still somewhat unstable and no direct release are offered,
however, unofficial nightly builds exist for both Linux and Windows `at MITB.com
<http://www.moparisthebest.com/downloads/simba/>`_.

Previous releases
-----------------

Look at this link_ for older releases of Simba.

.. _link: http://simba.villavu.com/bin/Release/

.. _documentation-ref:


What's next?
------------

A good guide on how to continue is found `on Simba's documentation
<http://docs.villavu.com/simba/gettingstarted.html>`_.


Documentation
=============

The documentation_ contains a lot of valuable information about Simba and
is essential for both the starting and advanced programmer. It contains
tutorials, API references and design documentation.

.. _source:

Source code
===========

The Source code is hosted on github_, and can be cloned like this:

.. code-block:: bash

    git clone git://github.com/MerlijnWajer/Simba.git

Alternatively, there's also another web interface to the Simba repository, found
on `git.villavu.com <http://git.villavu.com/simba.git/>`_.

.. _github: https://github.com/MerlijnWajer/Simba

.. _bugs:

Bugs
====

Bugs should be reported at `bugs.villavu.com
<http://bugs.villavu.com/>`_.

.. _tools:

Tools
=====

Tools can be found `here <http://simba.villavu.com/bin/Tools/>`_. For now
there's only OCRBench, a program to test and debug Simba's OCR.

..
    Indices and tables
    ==================
    * :ref:`genindex`
    * :ref:`modindex`
    * :ref:`search`

