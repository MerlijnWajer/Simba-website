.. _releases:

Simba Releases
==============

The current stable release is Simba *0.97.4*.
See :ref:`download` to get it.

Simba 0.99 (Stable Release)
---------------------------

Current: Simba 0.99

Download: `Simba-0.99
<http://simba.villavu.com/bin/Release/0.99/SimbaInstaller.exe>`_.

Changes since 0.98 include:

-   Automatic Simba updates. (Can be disabled in the new Settings form)
-   Updated SRL updaters. (Will now properly install plugins when they are already in use)
-   DeleteFile, RenameFile added. (They are not sandboxed in Extensions)
-   SetPersistentMemory support in TMufasaBitmap. (For the new SMART)
-   FData is now exported for each TMufasaBitmap. This means you can directly access the memory from Lape and Plugins. You can also pass the FData pointer around in PascalScript. The type of FData differs per cpu. It's a 32 bit integer on 32 bit Simba, and a 64 bit integer on 64 bit Simba. (Just use a C 'long')
-   Installer ships with PDF and HTML documentation. (See the folder Documentation/ in your Simba folder)
-   libFFI is statically linked in all Simba's except the 64 bit Windows one.
-   CPascal disabled. RUTIS and CPascal support will be removed from the source soon.
-   New Settings Form. (*Tools -> Settings*])
-   Linux now properly shows current active interpreter.
-   Linux mouse input now works properly again.
-   Plugin backend rework; support for multiple ABIs.
-   Support for plugins in lape.
-   Latest and greatest Lape. You can now run most SRL scripts on Linux and Windows.
-   Simba is portable by default. If a system wide install is required by some users, this can be arranged.
-   The non-portable version of Simba now respects user directories on both Windows and Unix (with XDG support).
-   More hash/cipher functions.
-   SQLite support. (If the sqlite3 library is available)
-   Major settings backend rework.
-   Added Version to Simba's UserAgent.
-   Support for JPG/PNG in TMufasaBitmap.SaveToFile (and in SaveBitmap)
-   Formatter extension to nicely format your scripts.
-   Examples/ directory.
-   SendKeys now also has **keymodwait**
-   **onScriptOpen** and **onScriptStart** hooks for extensions.
-   Crash logger. When something goes wrong, Simba will attempt to write a log to a file. You can then choose to keep running Simba or terminate it. (*I feel this is the most experimental feature*)
-   Initial support for loading a bitmap from clipboard in the bitmap convertor.

Bugs fixed:


-    http://bugs.villavu.com/view.php?id=404: Ctrl + Space Function List,, Make it Resizeable
-    http://bugs.villavu.com/view.php?id=409: Warning @ no memory manager set
-    http://bugs.villavu.com/view.php?id=406: BitmapExists()
-    http://bugs.villavu.com/view.php?id=408: DTM is inconsistent (Simba 990+)
-    http://bugs.villavu.com/view.php?id=400: Ini files aren't secure
-    http://bugs.villavu.com/view.php?id=127: SQLite for Simba?
-    http://bugs.villavu.com/view.php?id=403: Path Constants
-    http://bugs.villavu.com/view.php?id=402: ScriptFile
-    http://bugs.villavu.com/view.php?id=382: Suggestion: Add X button to function list to quickly clear searches.
-    http://bugs.villavu.com/view.php?id=380: FindColoredAreaTolerance
-    http://bugs.villavu.com/view.php?id=379: Error
-    http://bugs.villavu.com/view.php?id=378: glitchy
-    http://bugs.villavu.com/view.php?id=375: MSI: couldn't find MSI
-    http://bugs.villavu.com/view.php?id=373: CPU management
-    http://bugs.villavu.com/view.php?id=370: Control + Space broken.
-    http://bugs.villavu.com/view.php?id=360: Script formatter?
-    http://bugs.villavu.com/view.php?id=314: Settings.xml should be written more often
-    http://bugs.villavu.com/view.php?id=293: Add a Report Window to Simba
-    http://bugs.villavu.com/view.php?id=292: Simba needs a portable installer
-    http://bugs.villavu.com/view.php?id=266: Missing functions ( I dont know if syntax is changed from scar.)
-    http://bugs.villavu.com/view.php?id=263: Change font in settings
-    http://bugs.villavu.com/view.php?id=255: Trouble with INI functions
-    http://bugs.villavu.com/view.php?id=247: out of ranges
-    http://bugs.villavu.com/view.php?id=224: Change the way file specific conditionals are defined.
-    http://bugs.villavu.com/view.php?id=221: Change the way non-string settings are loaded
-    http://bugs.villavu.com/view.php?id=040: The Setting Form is Ugly
-    http://bugs.villavu.com/view.php?id=369: TFontStyle, fsUnderline = fsStrikeout, vice versa.
-    http://bugs.villavu.com/view.php?id=363: Ctrl+A in Debug Box = Ctrl+A on Script Typing Spot
-    http://bugs.villavu.com/view.php?id=280: TMDTM.AddPoint now returns the points index.
-    http://bugs.villavu.com/view.php?id=283: Length(s); and GetArrayLength(var arr);
-    http://bugs.villavu.com/view.php?id=251: Custom XML files
-    http://bugs.villavu.com/view.php?id=294: %HOMEDRIVE%\Simba\
-    http://bugs.villavu.com/view.php?id=305: Rearranged the Class registration (PascalScript) to fix a few problems.
-    http://bugs.villavu.com/view.php?id=366: Sum64IntArr
-    http://bugs.villavu.com/view.php?id=338: Can only load bitmap from file (no copy/paste)
-    http://bugs.villavu.com/view.php?id=415: Mouse support on Linux fixed.



Simba 0.98 (Stable Release)
---------------------------

Download: `Simba-0.98.2
<http://simba.villavu.com/bin/Release/0.98.2/SimbaInstaller.exe>`_.

Changes since 0.97:

-	TMFinder rewrite, including CTS support in all Find* functions.
-	CTS 3.
-	Updated Extensions.
-	Memory Manager Setting for Plugins.
-	Lape experimental support.
-	SendKeys now takes a wait parameter.
-	Exported SIMBA<VERSION> and SIMBAMAJOR<VERSION>.
-	Fixed WARNING/ERROR/LOADLIB directives inside conditionals.
-	Fixed a small bug in OCR loading.
-	Renamed ps_Tan to Tan.
-	Exported TMufasaBitmap.LoadFromTBitmap.
-	Added TWinControl.DoubleBuffered
-	DTM Editor fixes.
-	Removed Find*Optimised functions.
-	Various documentation changes.

Bugs fixed:


- http://bugs.villavu.com/view.php?id=359
- http://bugs.villavu.com/view.php?id=357
- http://bugs.villavu.com/view.php?id=355
- http://bugs.villavu.com/view.php?id=352
- http://bugs.villavu.com/view.php?id=349
- http://bugs.villavu.com/view.php?id=342
- http://bugs.villavu.com/view.php?id=341
- http://bugs.villavu.com/view.php?id=334
- http://bugs.villavu.com/view.php?id=331
- http://bugs.villavu.com/view.php?id=324
- http://bugs.villavu.com/view.php?id=321
- http://bugs.villavu.com/view.php?id=215
- http://bugs.villavu.com/view.php?id=313
- http://bugs.villavu.com/view.php?id=297
- http://bugs.villavu.com/view.php?id=309
- http://bugs.villavu.com/view.php?id=222



Simba 0.97 (Stable Release)
---------------------------


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

