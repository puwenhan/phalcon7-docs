Class **Phalcon\\Debug**
========================

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/debug.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Provides debug capabilities to Phalcon applications


Methods
-------

public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **setUri** (*string* $uri)

Change the base URI for static resources



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **setShowBackTrace** (*boolean* $showBackTrace)

Sets if files the exception's backtrace must be showed



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **setShowFiles** (*boolean* $showFiles)

Set if files part of the backtrace must be shown in the output



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **setShowFileFragment** (*boolean* $showFileFragment)

Sets if files must be completely opened and showed in the output or just the fragment related to the exception



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **listen** ([*boolean* $exceptions], [*boolean* $lowSeverity])

Listen for uncaught exceptions and unsilent notices or warnings



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **listenExceptions** ()

Listen for uncaught exceptions



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **listenLowSeverity** ()

Listen for unsilent notices or warnings or user-defined error



public  **halt** ()

Halts the request showing a backtrace



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **debugVar** (*mixed* $var, [*string* $key])

Adds a variable to the debug output



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **clearVars** ()

Clears are variables added previously



protected *string*  **_escapeString** ()

Escapes a string with htmlentities



protected *string*  **_getArrayDump** ()

Produces a recursive representation of an array



protected *string*  **_getVarDump** ()

Produces an string representation of a variable



public *string*  **getMajorVersion** ()

Returns the major framework's version



public *string*  **getVersion** ()

Generates a link to the current version documentation



public *string*  **getCssSources** ()

Returns the css sources



public *string*  **getJsSources** ()

Returns the javascript sources



protected  **showTraceItem** ()

Shows a backtrace item



public *boolean*  **onUncaughtException** (*\Exception* $exception)

Handles uncaught exceptions



public *boolean*  **onUserDefinedError** (*int* $severity, *string* $message, [*string* $file], [*string* $line], [*array* $context])

Handles user-defined error



public *boolean*  **onShutdown** ()

Handles user-defined error



public *int*  **getLinesBeforeContext** ()

Returns the number of lines deplayed before the error line



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **setLinesBeforeContext** (*int* $lines)

Sets the number of lines deplayed before the error line



public *int*  **getLinesAfterContext** ()

Returns the number of lines deplayed after the error line



public :doc:`Phalcon\\Debug <Phalcon_Debug>`  **setLinesAfterContext** (*int* $lines)

Sets the number of lines deplayed after the error line



protected  **getFileLink** (*unknown* $file, *unknown* $line, *unknown* $format)

...


public static  **enable** ([:doc:`Phalcon\\Logger\\AdapterInterface <Phalcon_Logger_AdapterInterface>` $logger])

Enable simple debug mode



public static  **disable** ()

Disable simple debug mode



public static  **log** (*string* $message, [*mixed* $type], [*array* $context])

Logs messages



