Class **Phalcon\\CLI\\Dispatcher**
==================================

*extends* abstract class :doc:`Phalcon\\Dispatcher <Phalcon_Dispatcher>`

*implements* :doc:`Phalcon\\DispatcherInterface <Phalcon_DispatcherInterface>`, :doc:`Phalcon\\DI\\InjectionAwareInterface <Phalcon_DI_InjectionAwareInterface>`, :doc:`Phalcon\\Events\\EventsAwareInterface <Phalcon_Events_EventsAwareInterface>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/cli/dispatcher.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Dispatching is the process of taking the command-line arguments, extracting the module name, task name, action name, and optional parameters contained in it, and then instantiating a task and calling an action on it.  

.. code-block:: php

    <?php

    $di = new Phalcon\DI();
    
    $dispatcher = new Phalcon\CLI\Dispatcher();
    
      $dispatcher->setDI($di);
    
    $dispatcher->setTaskName('posts');
    $dispatcher->setActionName('index');
    $dispatcher->setParams(array());
    
    $handle = $dispatcher->dispatch();



Constants
---------

*integer* **EXCEPTION_NO_DI**

*integer* **EXCEPTION_CYCLIC_ROUTING**

*integer* **EXCEPTION_HANDLER_NOT_FOUND**

*integer* **EXCEPTION_INVALID_HANDLER**

*integer* **EXCEPTION_INVALID_PARAMS**

*integer* **EXCEPTION_ACTION_NOT_FOUND**

Methods
-------

public  **setTaskSuffix** (*string* $taskSuffix)

Sets the default task suffix



public  **setDefaultTask** (*string* $taskName)

Sets the default task name



public  **setTaskName** (*string* $taskName)

Sets the task name to be dispatched



public *string*  **getTaskName** ()

Gets last dispatched task name



protected  **_throwDispatchException** ()

Throws an internal exception



protected  **_handleException** ()

Handles a user exception



public *string*  **getTaskClass** ()

Possible task class name that will be located to dispatch the request



public :doc:`Phalcon\\CLI\\Task <Phalcon_CLI_Task>`  **getLastTask** ()

Returns the lastest dispatched controller



public :doc:`Phalcon\\CLI\\Task <Phalcon_CLI_Task>`  **getActiveTask** ()

Returns the active task in the dispatcher



public  **__construct** () inherited from Phalcon\\Dispatcher

Phalcon\\Dispatcher constructor



public  **setActionSuffix** (*string* $actionSuffix) inherited from Phalcon\\Dispatcher

Sets the default action suffix



public  **setModuleName** (*string* $moduleName) inherited from Phalcon\\Dispatcher

Sets the module where the controller is (only informative)



public *string*  **getModuleName** () inherited from Phalcon\\Dispatcher

Gets the module where the controller class is



public  **setNamespaceName** (*string* $namespaceName) inherited from Phalcon\\Dispatcher

Sets the namespace where the controller class is



public *string*  **getNamespaceName** () inherited from Phalcon\\Dispatcher

Gets a namespace to be prepended to the current handler name



public  **setDefaultNamespace** (*string* $namespace) inherited from Phalcon\\Dispatcher

Sets the default namespace



public *string*  **getDefaultNamespace** () inherited from Phalcon\\Dispatcher

Returns the default namespace



public  **setDefaultAction** (*string* $actionName) inherited from Phalcon\\Dispatcher

Sets the default action name



public  **setActionName** (*string* $actionName) inherited from Phalcon\\Dispatcher

Sets the action name to be dispatched



public *string*  **getActionName** () inherited from Phalcon\\Dispatcher

Gets the lastest dispatched action name



public  **setLogicBinding** (*boolean* $value) inherited from Phalcon\\Dispatcher

Enable/Disable logic binding during dispatch



public *boolean*  **isLogicBinding** () inherited from Phalcon\\Dispatcher

Check if logic binding



public  **setParams** (*array* $params) inherited from Phalcon\\Dispatcher

Sets action params to be dispatched



public *array*  **getParams** () inherited from Phalcon\\Dispatcher

Gets action params



public  **setParam** (*mixed* $param, *mixed* $value) inherited from Phalcon\\Dispatcher

Set a param by its name or numeric index



public *mixed*  **getParam** (*mixed* $param, [*string|array* $filters]) inherited from Phalcon\\Dispatcher

Gets a param by its name or numeric index



public *string*  **getActiveMethod** () inherited from Phalcon\\Dispatcher

Returns the current method to be/executed in the dispatcher



public *boolean*  **isFinished** () inherited from Phalcon\\Dispatcher

Checks if the dispatch loop is finished or has more pendent controllers/tasks to disptach



public  **setFinished** (*boolean* $finished) inherited from Phalcon\\Dispatcher

Sets the finished



public  **setReturnedValue** (*mixed* $value) inherited from Phalcon\\Dispatcher

Sets the latest returned value by an action manually



public *mixed*  **getReturnedValue** () inherited from Phalcon\\Dispatcher

Returns value returned by the lastest dispatched action



public *object*  **dispatch** () inherited from Phalcon\\Dispatcher

Dispatches a handle action taking into account the routing parameters



public *bool*  **forward** (*string|array* $forward) inherited from Phalcon\\Dispatcher

Forwards the execution flow to another controller/action Dispatchers are unique per module. Forwarding between modules is not allowed 

.. code-block:: php

    <?php

      $this->dispatcher->forward(array('controller' => 'posts', 'action' => 'index'));




public *boolean*  **wasForwarded** () inherited from Phalcon\\Dispatcher

Check if the current executed action was forwarded by another one



public *string*  **getHandlerClass** () inherited from Phalcon\\Dispatcher

Possible class name that will be located to dispatch the request



public  **camelizeNamespace** (*bool* $camelize) inherited from Phalcon\\Dispatcher

Enables/Disables automatically camelize namespace  

.. code-block:: php

    <?php

      $this->dispatcher->camelizeNamespace(FALSE);




public  **camelizeController** (*bool* $camelize) inherited from Phalcon\\Dispatcher

Enables/Disables automatically camelize controller  

.. code-block:: php

    <?php

      $this->dispatcher->camelizeController(FALSE);




public :doc:`Phalcon\\DispatcherInterface <Phalcon_DispatcherInterface>`  **setErrorHandler** (*unknown* $callback, [*int* $exception_code]) inherited from Phalcon\\Dispatcher

Set error handler



public *mixed*  **getErrorHandler** (*int* $exception_code) inherited from Phalcon\\Dispatcher

Get error handler



public *boolean*  **fireEvent** (*string* $eventName, [*string* $data], [*string* $cancelable]) inherited from Phalcon\\Dispatcher

Fires an event, implicitly calls behaviors and listeners in the events manager are notified



public  **setDI** (:doc:`Phalcon\\DIInterface <Phalcon_DIInterface>` $dependencyInjector) inherited from Phalcon\\DI\\Injectable

Sets the dependency injector



public :doc:`Phalcon\\DIInterface <Phalcon_DIInterface>`  **getDI** ([*unknown* $error], [*unknown* $notUseDefault]) inherited from Phalcon\\DI\\Injectable

Returns the internal dependency injector



public  **setEventsManager** (:doc:`Phalcon\\Events\\ManagerInterface <Phalcon_Events_ManagerInterface>` $eventsManager) inherited from Phalcon\\DI\\Injectable

Sets the event manager



public :doc:`Phalcon\\Events\\ManagerInterface <Phalcon_Events_ManagerInterface>`  **getEventsManager** () inherited from Phalcon\\DI\\Injectable

Returns the internal event manager



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


