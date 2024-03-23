## Microservice decomposition strategy by vertical slices
Instead of breaking down features horizontally (across layers), you can break them down vertically, each representing an end-to-end slice of functionality. This way, each microservice encapsulates all the layers necessary to implement a specific feature.

Microservices are supposed to encapsulate business capabilities. A serivce representes a vertical slice and its composed by horizontal slices. Meaning the features and functionalities within the business capability is encapsulated into a service.

Depending on complexity, this vertical slice might represent different levels. Being them: capabilities, sub-business capabilities, features, or functionalities.


When decomposing your system, you start with higher-level concepts such as business capabilities, sub-business capabilities, features, or functionalities. For each of these, you evaluate the complexity and scope. If the complexity and scope are suitable for encapsulation within a single service, you stop there and create a microservice to implement that functionality.

However, if the complexity and scope are too large for a single service, you continue breaking down the functionality into smaller units, moving down the hierarchy. This process continues until you reach a level where the complexity and scope are manageable for a single service, typically at the level of a functionality or a smaller unit of work.

By following this approach, you ensure that each microservice has a clear and well-defined purpose, encapsulating a cohesive set of functionality. This promotes modularity, scalability, and maintainability in your system architecture.



