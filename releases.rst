.. _releases:

Simba Releases
==============

The current stable release is Simba 0.96.
See :ref:`download` to get it.

.. _simba-0.97-rc4:

Simba 0.97-rc4 (Development Release)
------------------------------------

Download: `Simba -0.97-rc4
<http://simba.villavu.com/bin/Release/0.97-rc4/SimbaInstaller.exe>`_.

Changes since the stable release include (but are not limited to!):

    -   `WARNING and ERROR directives`_
    -   Initial `External Editor <http://docs.villavu.com/simba/features/ui.html#read-only-external-editor-mode>`_ / Read-Only mode support.
    -   Added two global keybindings. Ctrl+Alt+R and Ctrl+Alt+P. Their effect is starting the script and launching the colour picker, respectively.
    -   Started work to make Simba more modular.
    -   Documentation updates.
        (  special thanks to `Echo_ <http://villavu.com/forum/showpost.php?p=788000&postcount=2>`_ )

Bugs fixed:

    -   Memory clean-ups and fixes.
    -   Updater form no longer shows when there is no update.
    -   Fix tab closing via 'x' on Widget sets other than win32.
    -   Fix include_once.
    -   Disguise also changes the name of the application now.
    -   Console is hidden by default.
    -   StrToInt raises an exception on invalid string.
        ( Resolves `Bug #298 <http://bugs.villavu.com/view.php?id=298>`_ )
    -   Allow CTS 2 for bitmaps.
        ( Resolves `Bug #297 <http://bugs.villavu.com/view.php?id=297>`_ )
    -   Change UK/US language usage inconsistency.
        ( Resolves `Bug #296 <http://bugs.villavu.com/view.php?id=296>`_ )
    -   Keyboard layout is not properly used in SendKey/SendString
        ( Resolves `Bug #307 <http://bugs.villavu.com/view.php?id=307>`_,
        `Bug #299 <http://bugs.villavu.com/view.php?id=299>`_ and
        `Bug #288 <http://bugs.villavu.com/view.php?id=288>`_ )
    -   Added Log10, even though we already had LogN.
    -   Extension updates, mainly to the paster extension.

Installer notes:

    -   Removed Fonts/ from the installer.
    -   Removes Tests/PS from the installer.
    -   Security extension doesn't seem to compile at the moment.


WARNING and ERROR directives
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: pascal

    {$WARNING This division doesn't work when the number is 0...}
    x := 42/ number;

.. code-block:: pascal

    {$IFDEF WINDOWS}
    {$ERROR Windows is not supported} //This will stop the compilation
    {$ENDIF}




Simba 0.96 (Stable Release)
---------------------------

Download: `Simba -0.96
<http://simba.villavu.com/bin/Release/0.96rc/SimbaInstaller.exe>`_.

Changes:

    -   Plugins can now export types.
    -   Socket support.
    -   GetProc/FindWindow functionality.
    -   More hashing functions.

