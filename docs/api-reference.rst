API Reference
=============
xtuml
-----
The following section lists functions, classes and exceptions from the xtuml 
module. The operations are independent of the underlying metamodel definition, 
i.e. the sql schema.

Loading Metaodels
^^^^^^^^^^^^^^^^^
.. autofunction:: xtuml.load_metamodel

.. autoclass:: xtuml.ModelLoader
   :members: build_metamodel, file_input, filename_input, input, populate

.. autoclass:: xtuml.UUIDGenerator

.. autoclass:: xtuml.IntegerGenerator



Metamodel Operations
^^^^^^^^^^^^^^^^^^^^
.. autoclass:: xtuml.MetaModel
   :members: clone, new, select_one, select_many

.. autofunction:: xtuml.delete
.. autofunction:: xtuml.navigate_one
.. autofunction:: xtuml.navigate_any
.. autofunction:: xtuml.navigate_many
.. autofunction:: xtuml.navigate_subtype
.. autofunction:: xtuml.relate
.. autofunction:: xtuml.unrelate
.. autofunction:: xtuml.where_eq

.. autofunction:: xtuml.check_association_integrity

Persistance
^^^^^^^^^^^
.. autofunction:: xtuml.persist_database
.. autofunction:: xtuml.persist_instances
.. autofunction:: xtuml.persist_schema

.. autofunction:: xtuml.serialize
.. autofunction:: xtuml.serialize_database
.. autofunction:: xtuml.serialize_schema
.. autofunction:: xtuml.serialize_instances
.. autofunction:: xtuml.serialize_instance

Exceptions
^^^^^^^^^^
.. autoexception:: xtuml.ParsingException
.. autoexception:: xtuml.ModelException


bridgepoint
-----------
The following section lists functions and classes from the bridgepoint module. 
All operations require input expressed in the BridgePoint metamodel (ooaofooa).

Loading Models
^^^^^^^^^^^^^^
.. autofunction:: bridgepoint.load_model

.. autoclass:: bridgepoint.ModelLoader
   :members: filename_input

Model Transformation
^^^^^^^^^^^^^^^^^^^^
.. autofunction:: bridgepoint.gen_text_action
.. autofunction:: bridgepoint.prebuild_action
.. autofunction:: bridgepoint.prebuild_model

