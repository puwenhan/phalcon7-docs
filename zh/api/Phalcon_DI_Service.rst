Class **Phalcon\\DI\\Service**
==============================

*implements* :doc:`Phalcon\\DI\\ServiceInterface <Phalcon_DI_ServiceInterface>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/di/service.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Represents individually a service in the services container  

.. code-block:: php

    <?php

     $service = new Phalcon\DI\Service('request', 'Phalcon\Http\Request');
     $request = $service->resolve();

.. code-block:: php

    <?php



Methods
-------

public  **__construct** (*string* $name, *mixed* $definition, [*boolean* $shared])





public  **getName** ()

Returns the service's name



public  **setShared** (*boolean* $shared)

Sets if the service is shared or not



public *boolean*  **isShared** ()

Check whether the service is shared or not



public  **setSharedInstance** (*mixed* $sharedInstance)

Sets/Resets the shared instance related to the service



public  **setDefinition** (*mixed* $definition)

Set the service definition



public *mixed*  **getDefinition** ()

Returns the service definition



public *object*  **resolve** ([*array* $parameters], [:doc:`Phalcon\\DIInterface <Phalcon_DIInterface>` $dependencyInjector])

Resolves the service



public :doc:`Phalcon\\DI\\Service <Phalcon_DI_Service>`  **setParameter** (*long* $position, *array* $parameter)

Changes a parameter in the definition without resolve the service



public *array*  **getParameter** (*int* $position)

Returns a parameter in a specific position



public *boolean*  **isResolved** ()

Returns true if the service was resolved



public static :doc:`Phalcon\\DI\\Service <Phalcon_DI_Service>`  **__set_state** ([*array* $properties])

Restore the internal state of a service



