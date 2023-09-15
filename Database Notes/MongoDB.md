Here are some points to consider when deciding whether MongoDB would be a good fit:

Product Attributes and Variations: If your products have a variety of different attributes and variations, MongoDB can handle this well with its schema-less structure, which allows for great flexibility in data representation.

Relationships Between Entities: If your system design involves complex relationships between different entities (like products having multiple categories, dependencies, or hierarchical relationships), a relational database might offer more structured ways to handle these relationships with features like foreign keys and joins.

Query Patterns: Consider the types of queries you'll be executing most often. If they are mostly straightforward CRUD operations, MongoDB can be a great fit. If you anticipate needing to perform complex queries involving multiple joins, a relational database might be more efficient.

Data Integrity: If maintaining strict data integrity is a priority, a relational database might offer better support with its ACID properties. MongoDB can also maintain data integrity but might require more careful design and management, especially in the context of transactions.