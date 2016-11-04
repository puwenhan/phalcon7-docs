Class **Phalcon\\Mvc\\Model\\MetaData\\Strategy\\Annotations**
==============================================================

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/mvc/model/metadata/strategy/annotations.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Queries the table meta-data in order to instrospect the model's metadata


Methods
-------

public *array*  **getMetaData** (:doc:`Phalcon\\Mvc\\ModelInterface <Phalcon_Mvc_ModelInterface>` $model, :doc:`Phalcon\\DIInterface <Phalcon_DIInterface>` $dependencyInjector)

The meta-data is obtained by reading the column descriptions from the database information schema



public *array*  **getColumnMaps** ()

Read the model's column map, this can't be inferred



