Class **Phalcon\\Flash\\Session**
=================================

*extends* abstract class :doc:`Phalcon\\Flash <Phalcon_Flash>`

*implements* :doc:`Phalcon\\DI\\InjectionAwareInterface <Phalcon_DI_InjectionAwareInterface>`, :doc:`Phalcon\\Events\\EventsAwareInterface <Phalcon_Events_EventsAwareInterface>`, :doc:`Phalcon\\FlashInterface <Phalcon_FlashInterface>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/flash/session.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Temporarily stores the messages in session, then messages can be printed in the next request


Methods
-------

protected *array*  **_getSessionMessages** ()

Returns the messages stored in session



protected  **_setSessionMessages** ()

Stores the messages in session



public  **message** (*string* $type, *string* $message)

Adds a message to the session flasher



public *array*  **getMessages** ([*string* $type], [*boolean* $remove])

Returns the messages in the session flasher



public  **output** ([*string* $type], [*boolean* $remove])

Prints the messages in the session flasher



public  **has** (*unknown* $type)

bool \\Phalcon\\Flash\\Session::has(string $type)



public  **__construct** ([*array* $cssClasses]) inherited from Phalcon\\Flash

Phalcon\\Flash constructor



public :doc:`Phalcon\\FlashInterface <Phalcon_FlashInterface>`  **setImplicitFlush** (*boolean* $implicitFlush) inherited from Phalcon\\Flash

Set whether the output must be implictly flushed to the output or returned as string



public :doc:`Phalcon\\FlashInterface <Phalcon_FlashInterface>`  **setAutomaticHtml** (*boolean* $automaticHtml) inherited from Phalcon\\Flash

Set if the output must be implictily formatted with HTML



public :doc:`Phalcon\\FlashInterface <Phalcon_FlashInterface>`  **setCssClasses** (*array* $cssClasses) inherited from Phalcon\\Flash

Set an array with CSS classes to format the messages



public *string*  **error** (*string* $message) inherited from Phalcon\\Flash

Shows a HTML error message 

.. code-block:: php

    <?php

     $flash->error('This is an error');




public *string*  **notice** (*string* $message) inherited from Phalcon\\Flash

Shows a HTML notice/information message 

.. code-block:: php

    <?php

     $flash->notice('This is an information');




public *string*  **success** (*string* $message) inherited from Phalcon\\Flash

Shows a HTML success message 

.. code-block:: php

    <?php

     $flash->success('The process was finished successfully');




public *string*  **warning** (*string* $message) inherited from Phalcon\\Flash

Shows a HTML warning message 

.. code-block:: php

    <?php

     $flash->warning('Hey, this is important');




public  **outputMessage** (*string* $type, *string* $message) inherited from Phalcon\\Flash

Outputs a message formatting it with HTML 

.. code-block:: php

    <?php

     $flash->outputMessage('error', $message);




public  **setDI** (:doc:`Phalcon\\DIInterface <Phalcon_DIInterface>` $dependencyInjector) inherited from Phalcon\\DI\\Injectable

Sets the dependency injector



public :doc:`Phalcon\\DIInterface <Phalcon_DIInterface>`  **getDI** ([*unknown* $error], [*unknown* $notUseDefault]) inherited from Phalcon\\DI\\Injectable

Returns the internal dependency injector



public  **setEventsManager** (:doc:`Phalcon\\Events\\ManagerInterface <Phalcon_Events_ManagerInterface>` $eventsManager) inherited from Phalcon\\DI\\Injectable

Sets the event manager



public :doc:`Phalcon\\Events\\ManagerInterface <Phalcon_Events_ManagerInterface>`  **getEventsManager** () inherited from Phalcon\\DI\\Injectable

Returns the internal event manager



public *boolean*  **fireEvent** (*string* $eventName, [*unknown* $data], [*unknown* $cancelable]) inherited from Phalcon\\DI\\Injectable

Fires an event, implicitly calls behaviors and listeners in the events manager are notified



public *boolean*  **fireEventCancel** (*string* $eventName, [*unknown* $data], [*unknown* $cancelable]) inherited from Phalcon\\DI\\Injectable

Fires an event, implicitly calls behaviors and listeners in the events manager are notified This method stops if one of the callbacks/listeners returns boolean false



public *boolean*  **hasService** (*string* $name) inherited from Phalcon\\DI\\Injectable

Check whether the DI contains a service by a name



public *mixed*  **getResolveService** (*string* $name, [*unknown* $args], [*unknown* $noerror], [*unknown* $noshared]) inherited from Phalcon\\DI\\Injectable

Resolves the service based on its configuration



public  **__get** (*unknown* $property) inherited from Phalcon\\DI\\Injectable

Magic method __get



public  **__sleep** () inherited from Phalcon\\DI\\Injectable

...


public  **__debugInfo** () inherited from Phalcon\\DI\\Injectable

...


