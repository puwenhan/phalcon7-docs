Abstract class **Phalcon\\Mvc\\User\\Logic\\Model**
===================================================

*extends* abstract class :doc:`Phalcon\\Mvc\\User\\Logic <Phalcon_Mvc_User_Logic>`

*implements* :doc:`Phalcon\\DI\\InjectionAwareInterface <Phalcon_DI_InjectionAwareInterface>`, :doc:`Phalcon\\Events\\EventsAwareInterface <Phalcon_Events_EventsAwareInterface>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/mvc/user/logic/model.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Phalcon\\Mvc\\User\\Logic  This class can be used to provide user business logic an easy access to services in the application


Methods
-------

abstract public  **get** ([*unknown* $arguments])

...


abstract public  **getAll** ([*unknown* $arguments])

...


abstract public  **save** ([*unknown* $arguments])

...


abstract public  **create** ([*unknown* $arguments])

...


abstract public  **delete** ([*unknown* $arguments])

...


abstract public  **deleteAll** ([*unknown* $arguments])

...


abstract public  **update** ([*unknown* $arguments])

...


abstract public  **updateAll** ([*unknown* $arguments])

...


abstract public  **count** ([*unknown* $arguments])

...


public  **__construct** ([*string* $actionName], [*unknown* $arguments]) inherited from Phalcon\\Mvc\\User\\Logic

Constructor for Phalcon\\Mvc\\User\\Logic



public *string*  **getActionName** () inherited from Phalcon\\Mvc\\User\\Logic

Gets the action name



public *array*  **getActionParams** () inherited from Phalcon\\Mvc\\User\\Logic

Gets action params



public  **setContent** (*mixed* $content) inherited from Phalcon\\Mvc\\User\\Logic

Sets content



public *mixed*  **getContent** () inherited from Phalcon\\Mvc\\User\\Logic

Gets content



public static *object*  **call** ([*string* $actionName], [*unknown* $arguments]) inherited from Phalcon\\Mvc\\User\\Logic

Loads an logic and prepares it for manipulation



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


