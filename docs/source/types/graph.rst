================
Graph Data Types
================

Cypher queries can return entire graph structures as well as individual property values.

, The graph types model graph data returned from a Cypher query.
Graph values cannot be passed in as parameters as it would be unclear whether the entity was intended to be passed by reference or by value.
The identity or properties of that entity should be passed explicitly instead.

All graph values returned within a given :class:`.StatementResult` are contained within a :class:`.Graph` instance, accessible via :meth:`.StatementResult.graph`.
The driver contains a corresponding class for each of the graph types that can be returned.

=============  ======================
Cypher Type    Python Type
=============  ======================
Node           :class:`.Node`
Relationship   :class:`.Relationship`
Path           :class:`.Path`
=============  ======================

.. autoclass:: neo4j.v1.types.graph.Graph
   :members:

.. autoclass:: neo4j.v1.types.graph.Entity
   :members:

.. autoclass:: neo4j.v1.types.graph.EntitySetView
   :members:

.. autoclass:: neo4j.v1.types.graph.Node
   :members:
   :inherited-members:

.. autoclass:: neo4j.v1.types.graph.Relationship
   :members:
   :inherited-members:

.. autoclass:: neo4j.v1.types.graph.Path
   :members:
