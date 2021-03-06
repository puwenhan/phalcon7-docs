Abstract class **Phalcon\\Validation\\Validator**
=================================================

*implements* :doc:`Phalcon\\Validation\\ValidatorInterface <Phalcon_Validation_ValidatorInterface>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/validation/validator.c" class="btn btn-default btn-sm">Source on GitHub</a>`

This is a base class for validators


Methods
-------

public  **__construct** ([*array* $options])

Phalcon\\Validation\\Validator constructor



public *mixed*  **isSetOption** (*string* $key)

Checks if an option is defined



public *mixed*  **getOption** (*string* $key)

Returns an option in the validator's options Returns null if the option hasn't been set



public  **setOption** (*string* $key, *mixed* $value)

Sets an option in the validator



public *mixed*  **getType** ()

Gets an type in the validator



abstract public *boolean*  **validate** (*Phalcon\\Validator* $validator, *string* $attribute) inherited from Phalcon\\Validation\\ValidatorInterface

Executes the validation



abstract public *boolean*  **valid** () inherited from Phalcon\\Validation\\ValidatorInterface

Executes the validation



