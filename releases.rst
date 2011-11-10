.. _releases:

Simba Releases
==============

The current stable release is Simba *0.97.1*.
See :ref:`download` to get it.

Simba 0.97 (Stable Release)
---------------------------

Current: Simba 0.97.4

Download: `Simba-0.97.4
<http://simba.villavu.com/bin/Release/0.97.4/SimbaInstaller.exe>`_.

Changes since :ref:`simba-0.96` include (but are not limited to!):

    -   `WARNING and ERROR directives`_
    -   Initial `External Editor <http://docs.villavu.com/simba/features/ui.html#read-only-external-editor-mode>`_ / Read-Only mode support.
    -   Added two global keybindings. Ctrl+Alt+R and Ctrl+Alt+P. Their effect is starting the script and launching the colour picker, respectively.
    -   Documentation updates.
        (  special thanks to `Echo_ <http://villavu.com/forum/showpost.php?p=788000&postcount=2>`_ )
    -   Added ``extension.sex``, the Extension updater. (Make sure you enable it!)

Bugs fixed:

    -   Bug fixes to the DTM Editor Extension
    -   Added Plugin Memory Manager.
    -   SendKeys now supports keywait parameter.
        (Resolves `Bug #324 <http://bugs.villavu.com/view.php?id=324>`_ )
    -   Memory clean-ups and fixes.
    -   Started work to make Simba more modular.
    -   Added FilterTPACustom
    -   Updater form no longer shows when there is no update.
    -   Fix tab closing via 'x' on Widget sets other than win32.
    -   Fix *INCLUDE_ONCE*.
    -   Disguise also changes the name of the application now.
    -   Console is hidden by default.
    -   StrToInt raises an exception on invalid string.
        ( Resolves `Bug #298 <http://bugs.villavu.com/view.php?id=298>`_ )
        *Make sure you don't forget to use StrToIntDef if you want to keep the
        behaviour similar to the old StrToInt!*
    -   Allow CTS 2 for bitmaps.
        ( Resolves `Bug #297 <http://bugs.villavu.com/view.php?id=297>`_ )
    -   Change UK/US language usage inconsistency.
        ( Resolves `Bug #296 <http://bugs.villavu.com/view.php?id=296>`_ )
    -   Keyboard layout is now properly used in SendKey/SendString
        ( Resolves `Bug #307 <http://bugs.villavu.com/view.php?id=307>`_,
        `Bug #299 <http://bugs.villavu.com/view.php?id=299>`_ and
        `Bug #288 <http://bugs.villavu.com/view.php?id=288>`_ )
    -   HTTPS support when openssl is installed.
        (Resolves  `Bug #295 <http://bugs.villavu.com/view.php?id=295>`_ )
    -   Added Log10, even though we already had LogN.
    -   Extension updates, to the paster extension and a new extension: the
        extension updater. (``extension.sex``)
    -   Fix memory leak in FindBitmapSpiralTolerance (leak only effective on
        Linux)
    -   Settings constants `Bug #222 <http://bugs.villavu.com/view.php?id=222>`_ )
    -   Added DeleteFile `Bug #309 <http://bugs.villavu.com/view.php?id=309>`_ )
    -   ExtPath in Extensions works again.
    -   Fixed CopyPath declaration.
    -   Fixed Security Extension. `Bug #313 <http://bugs.villavu.com/view.php?id=313>`_
    -   Workaround for `Bug #316. <http://bugs.villavu.com/view.php?id=316>`_
        Causes a regression in codehints. (*Plugin functions are no longer shown*)
    -   Documentation additions. (TPA, MML)
    -   PointToBox parameters changed to be more clear.


Installer notes:

    -   Removed Fonts/ from the installer. (They are installed on launch anyway)
    -   Removes Tests/PS from the installer.
    -   Security extension doesn't seem to compile at the moment.
    -   Provided a default settings.xml which is both portable and enables the
        ``extension.sex`` extension by default.

WARNING and ERROR directives
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: pascal

    {$WARNING This division doesn't work when the number is 0...}
    x := 42 / number;

.. code-block:: pascal

    {$IFDEF WINDOWS}
    {$ERROR Windows is not supported} //This will stop the compilation
    {$ENDIF}



Simba 0.97-rc6 (Development Release)
------------------------------------

Download: `Simba-0.97-rc6
<http://simba.villavu.com/bin/Release/0.97-rc6/SimbaInstaller.exe>`_.

Simba 0.97-rc5 (Development Release)
------------------------------------

Download: `Simba-0.97-rc5
<http://simba.villavu.com/bin/Release/0.97-rc5/SimbaInstaller.exe>`_.

Simba 0.97-rc4 (Development Release)
------------------------------------

Download: `Simba-0.97-rc4
<http://simba.villavu.com/bin/Release/0.97-rc4/SimbaInstaller.exe>`_.


.. _simba-0.96:

Simba 0.96 (Old Stable Release)
-------------------------------

Download: `Simba-0.96
<http://simba.villavu.com/bin/Release/0.96rc/SimbaInstaller.exe>`_.

Changes:

    -   Plugins can now export types.
    -   Socket support.
    -   GetProc/FindWindow functionality.
    -   More hashing functions.

