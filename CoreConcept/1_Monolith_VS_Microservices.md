![image](https://github.com/chrahul/The_Art_of_Solution_Designing/assets/14847377/798b53d4-a3ad-4dc5-ad90-05958153c4b0)



### Monolith:

- **Definition**: A single-tier software application where the user interface and data access code are combined into a single program from a single platform.
- **Examples**: Single Java JAR file, COBOL program.
- **Advantages**:
  - Simplicity, especially for small projects.
  - Resource efficiency at small scale.
- **Challenges**:
  - Lack of modularity as the project grows.
  - Difficulty in enforcing scalability.
  - All-or-nothing deployment leading to long release cycles.
- **Integration with APIs**: Monolith can be fronted by API Gateway or load balancer to enable API usage.

![image](https://github.com/chrahul/The_Art_of_Solution_Designing/assets/14847377/eb779957-1917-4cc1-8a55-f6c2d2ef7dd3)



### Scaling Challenges with Monolith:

- Running on a virtual machine necessitates sizing for the entire application.
- Inefficient scaling as entire monolith must be scaled, even for specific components.
- Paying for resources not fully utilized.

### Microservices:

- **Definition**: Architecture where each component, or service, is independent, scalable, and deployed separately.
- **Characteristics**:
  - Independence of each service.
  - Scalability irrespective of others.
  - Different governance and security features.
  - Independent deployment.
- **Polyglot**: Different microservices can be written in different programming languages.
- **Example**: Store Slash Get, Store Slash Post, Store Slash Delete as separate microservices.
- **Advantages**:
  - Faster DevOps with independent deployments.
  - Testing and maintenance of services independent of each other.
- **Flexibility**: Can utilize shared databases but should optimize for increased connections.
- **Implementation**: 
  - Each microservice has its own codebase and runs on separate virtual machines.
  - Services can communicate via APIs or message brokers.
  - Can be implemented with different programming languages for each service.
- **Characteristics**:
  - Independence, scalability, and functional separation are key.
  - Not necessary to fulfill every microservice characteristic; flexibility is important.

This reference document should aid in preparing for system design interviews, particularly for Cloud Solution Architect roles.
