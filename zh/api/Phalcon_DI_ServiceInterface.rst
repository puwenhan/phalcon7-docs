Interface **Phalcon\\DI\\ServiceInterface**
===========================================

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/di/serviceinterface.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Phalcon\\DI\\ServiceInterface initializer


Methods
-------

abstract public *string*  **getName** ()

Returns the name of the service



abstract public  **setShared** (*boolean* $shared)

Sets whether the service is shared or not



abstract public *boolean*  **isShared** ()

Check whether the service is shared or not



abstract public  **setDefinition** (*mixed* $definition)

Set the service definition



abstract public *mixed*  **getDefinition** ()

Returns the service definition



abstract public *bool*  **isResolved** ()

Checks if the service was resolved



abstract public *object*  **resolve** ([*array* $parameters], [:doc:`Phalcon\\DIInterface <Phalcon_DIInterface>` $dependencyInjector])

Resolves the service



