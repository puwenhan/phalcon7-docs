Interface **Phalcon\\DIInterface**
==================================

*extends* ArrayAccess

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/diinterface.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Phalcon\\DIInterface initializer


Methods
-------

abstract public :doc:`Phalcon\\DI\\ServiceInterface <Phalcon_DI_ServiceInterface>`  **set** (*string* $name, *mixed* $definition, [*boolean* $shared])

Registers a service in the service container



abstract public  **remove** (*string* $name)

Removes a service from the service container



abstract public *object*  **get** (*string* $name, [*array* $parameters], [*boolean* $noError], [*unknown* $noerror])

Resolves the service based on its configuration



abstract public *object*  **getShared** (*string* $name, [*array* $parameters], [*boolean* $noError])

Resolves a shared service based on their configuration



abstract public :doc:`Phalcon\\DI\\ServiceInterface <Phalcon_DI_ServiceInterface>`  **setService** (*string* $name, :doc:`Phalcon\\DI\\ServiceInterface <Phalcon_DI_ServiceInterface>` $rawDefinition)

Sets a service using a raw Phalcon\\DI\\Service definition



abstract public :doc:`Phalcon\\DI\\ServiceInterface <Phalcon_DI_ServiceInterface>`  **getService** (*string* $name)

Returns the corresponding Phalcon\\Di\\Service instance for a service



abstract public *boolean*  **has** (*string* $name)

Check whether the DI contains a service by a name



abstract public *boolean*  **wasFreshInstance** ()

Check whether the last service obtained via getShared produced a fresh instance or an existing one



abstract public *array*  **getServices** ()

Return the services registered in the DI



abstract public static  **setDefault** (*Phalcon_DIInterface* $dependencyInjector)

Set the default dependency injection container to be obtained into static methods



abstract public static *Phalcon_DIInterface*  **getDefault** ()

Return the last DI created



abstract public static  **reset** ()

Resets the internal default DI



abstract public  **offsetExists** (*unknown* $offset) inherited from ArrayAccess

...


abstract public  **offsetGet** (*unknown* $offset) inherited from ArrayAccess

...


abstract public  **offsetSet** (*unknown* $offset, *unknown* $value) inherited from ArrayAccess

...


abstract public  **offsetUnset** (*unknown* $offset) inherited from ArrayAccess

...


