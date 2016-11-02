Class **Phalcon\\Db\\Dialect\\Mysql**
=====================================

*extends* abstract class :doc:`Phalcon\\Db\\Dialect <Phalcon_Db_Dialect>`

*implements* :doc:`Phalcon\\Db\\DialectInterface <Phalcon_Db_DialectInterface>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/db/dialect/mysql.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Generates database specific SQL for the MySQL RBDMS


Methods
-------

public *string*  **getColumnDefinition** (:doc:`Phalcon\\Db\\ColumnInterface <Phalcon_Db_ColumnInterface>` $column)

Gets the column name in MySQL



public *string*  **addColumn** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\ColumnInterface <Phalcon_Db_ColumnInterface>` $column)

Generates SQL to add a column to a table



public *string*  **modifyColumn** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\ColumnInterface <Phalcon_Db_ColumnInterface>` $column, [*unknown* $currentColumn])

Generates SQL to modify a column in a table



public *string*  **dropColumn** (*string* $tableName, *string* $schemaName, *string* $columnName)

Generates SQL to delete a column from a table



public *string*  **addIndex** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\IndexInterface <Phalcon_Db_IndexInterface>` $index)

Generates SQL to add an index to a table



public *string*  **dropIndex** (*string* $tableName, *string* $schemaName, *string* $indexName)

Generates SQL to delete an index from a table



public *string*  **addPrimaryKey** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\IndexInterface <Phalcon_Db_IndexInterface>` $index)

Generates SQL to add the primary key to a table



public *string*  **dropPrimaryKey** (*string* $tableName, *string* $schemaName)

Generates SQL to delete primary key from a table



public *string*  **addForeignKey** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\ReferenceInterface <Phalcon_Db_ReferenceInterface>` $reference)

Generates SQL to add an index to a table



public *string*  **dropForeignKey** (*string* $tableName, *string* $schemaName, *string* $referenceName)

Generates SQL to delete a foreign key from a table



protected *array*  **_getTableOptions** ()

Generates SQL to add the table creation options



public *string*  **createTable** (*string* $tableName, *string* $schemaName, *array* $definition)

Generates SQL to create a table in MySQL



public *string*  **dropTable** (*string* $tableName, *string* $schemaName)

Generates SQL to drop a table



public *string*  **createView** (*string* $viewName, *array* $definition, *string* $schemaName)

Generates SQL to create a view



public *string*  **dropView** (*string* $viewName, *string* $schemaName, [*boolean* $ifExists])

Generates SQL to drop a view



public *string*  **tableExists** (*string* $tableName, [*string* $schemaName])

Generates SQL checking for the existence of a schema.table 

.. code-block:: php

    <?php

     echo $dialect->tableExists("posts", "blog");
     echo $dialect->tableExists("posts");




public *string*  **viewExists** (*string* $viewName, [*string* $schemaName])

Generates SQL checking for the existence of a schema.view



public *string*  **describeColumns** (*string* $table, [*string* $schema])

Generates SQL describing a table 

.. code-block:: php

    <?php

    print_r($dialect->describeColumns("posts")) ?>




public *string*  **listTables** ([*string* $schemaName])

Generates SQL list all tables on database 

.. code-block:: php

    <?php

    print_r($dialect->listTables("blog")) ?>




public *string*  **listViews** ([*string* $schemaName])

Generates the SQL to list all views of a schema or user



public *string*  **describeIndexes** (*string* $table, [*string* $schema])

Generates SQL to query indexes on a table



public *string*  **describeReferences** (*string* $table, [*string* $schema])

Generates SQL to query foreign keys on a table



public *string*  **tableOptions** (*string* $table, [*string* $schema])

Generates the SQL to describe the table creation options



public *string*  **limit** (*string* $sqlQuery, *int* $number) inherited from Phalcon\\Db\\Dialect

Generates the SQL for LIMIT clause 

.. code-block:: php

    <?php

     $sql = $dialect->limit('SELECT * FROM robots', 10);
     echo $sql; // SELECT * FROM robots LIMIT 10




public *string*  **forUpdate** (*string* $sqlQuery) inherited from Phalcon\\Db\\Dialect

Returns a SQL modified with a FOR UPDATE clause 

.. code-block:: php

    <?php

     $sql = $dialect->forUpdate('SELECT * FROM robots');
     echo $sql; // SELECT * FROM robots FOR UPDATE




public *string*  **sharedLock** (*string* $sqlQuery) inherited from Phalcon\\Db\\Dialect

Returns a SQL modified with a LOCK IN SHARE MODE clause 

.. code-block:: php

    <?php

     $sql = $dialect->sharedLock('SELECT * FROM robots');
     echo $sql; // SELECT * FROM robots LOCK IN SHARE MODE




public *string*  **getColumnList** (*array* $columnList) inherited from Phalcon\\Db\\Dialect

Gets a list of columns with escaped identifiers 

.. code-block:: php

    <?php

     echo $dialect->getColumnList(array('column1', 'column'));




public *string*  **getSqlExpression** (*unknown* $expression, [*unknown* $escapeChar], [*unknown* $quoting]) inherited from Phalcon\\Db\\Dialect

Transforms an intermediate representation for a expression into a database system valid expression



public *string*  **getSqlExpressionCase** (*unknown* $expression, [*unknown* $escapeChar]) inherited from Phalcon\\Db\\Dialect

Resolve CASE expressions



public *string*  **getSqlExpressionFunctionCall** (*unknown* $expression, [*unknown* $escapeChar]) inherited from Phalcon\\Db\\Dialect

Resolve function calls



public *string*  **getSqlTable** (*array* $table, [*string* $escapeChar]) inherited from Phalcon\\Db\\Dialect

Transform an intermediate representation for a schema/table into a database system valid expression



public *string*  **select** (*array* $definition) inherited from Phalcon\\Db\\Dialect

Builds a SELECT statement



public *string*  **insert** (*array* $definition) inherited from Phalcon\\Db\\Dialect

Builds a INSERT statement



public *string*  **update** (*array* $definition, [*unknown* $quoting]) inherited from Phalcon\\Db\\Dialect

Builds a UPDATE statement



public *string*  **delete** (*array* $definition) inherited from Phalcon\\Db\\Dialect

Builds a DELETE statement



public *boolean*  **supportsSavepoints** () inherited from Phalcon\\Db\\Dialect

Checks whether the platform supports savepoints



public *boolean*  **supportsReleaseSavepoints** () inherited from Phalcon\\Db\\Dialect

Checks whether the platform supports releasing savepoints.



public *string*  **createSavepoint** (*string* $name) inherited from Phalcon\\Db\\Dialect

Generate SQL to create a new savepoint



public *string*  **releaseSavepoint** (*string* $name) inherited from Phalcon\\Db\\Dialect

Generate SQL to release a savepoint



public *string*  **rollbackSavepoint** (*string* $name) inherited from Phalcon\\Db\\Dialect

Generate SQL to rollback a savepoint



public *string*  **getEscapeChar** () inherited from Phalcon\\Db\\Dialect

Return the escape char



public *array*  **registerCustomFunction** (*unknown* $name, *unknown* $customFunction) inherited from Phalcon\\Db\\Dialect

Registers custom SQL functions



public *array*  **getCustomFunctions** () inherited from Phalcon\\Db\\Dialect

Returns registered functions



public *string*  **escape** (*string* $str, [*string* $escapeChar]) inherited from Phalcon\\Db\\Dialect

Escape identifiers



public *string*  **escapeSchema** (*string* $schema, [*string* $escapeChar]) inherited from Phalcon\\Db\\Dialect

Escape Schema



public *string*  **prepareTable** (*string* $table, [*string* $schema], [*string* $alias], [*string* $escapeChar]) inherited from Phalcon\\Db\\Dialect

Prepares table for this RDBMS



