---
aliases:
  - Project Template
Author: Atharva Chavan
Created: 2025-02-22
Updated: 
tags:
  - ProjectPlan
Comments:
---

# Project Template

## Overview
- This project involves building a simple multi-microservices project using GO Lang 
- Requirements : 
	- GO
	- gRPC
	- GraphQL
	- Docker
	- PostgreSQL
	- Elasticsearch
	- Microservices
- Challenges :
	- Complexity of Microservices
- 

## Goals

*   **Month 1: Go Fundamentals and Account Microservice**
    *   Goal 1:  Go Basics and gRPC Setup
        *   Learn Go syntax and basic programming concepts.
        *   Set up a gRPC development environment.
        *   Create a simple "Hello, World!" gRPC service.
    *   Goal 2: Account Microservice - Database and gRPC Interface
        *   Set up a PostgreSQL database for the account service[1].
        *   Define the account service gRPC interface using Protocol Buffers.
        *   Implement the gRPC server for the account service (create, read, update, delete accounts).
    *   Goal 3:  Dockerize Account Microservice
        *   Create a Dockerfile for the account microservice.
        *   Build and run the account microservice in a Docker container.
*   **Month 2: Product Microservice and GraphQL Gateway**
    *   Goal 4: Product Microservice - Elasticsearch and gRPC
        *   Set up Elasticsearch for the product service[1].
        *   Define the product service gRPC interface.
        *   Implement the gRPC server for the product service (create, read, update, delete products).
    *   Goal 5: Dockerize Product Microservice
        *   Create a Dockerfile for the product microservice.
        *   Build and run the product microservice in a Docker container.
    *   Goal 6: GraphQL Gateway Setup
        *   Set up a GraphQL server using a library like gqlgen[1].
        *   Define GraphQL queries and mutations for accounts and products.
        *   Implement resolvers that call the account and product gRPC services.
*   **Month 3: Order Microservice and Docker Compose**
    *   Goal 7: Order Microservice - PostgreSQL and gRPC
        *   Set up a PostgreSQL database for the order service[1].
        *   Define the order service gRPC interface.
        *   Implement the gRPC server for the order service (create, read, update, delete orders).  This service will need to interact with both the account and product microservices[1].
    *   Goal 8: Dockerize Order Microservice
        *   Create a Dockerfile for the order microservice.
        *   Build and run the order microservice in a Docker container.
    *   Goal 9: Docker Compose Integration
        *   Create a `docker-compose.yaml` file to define all microservices, databases, and the GraphQL gateway[1].
        *   Run the entire application using Docker Compose.
*   **Month 4: Testing, Refinement, and Deployment Basics**
    *   Goal 10:  Implement Unit and Integration Tests
        *   Write unit tests for each microservice.
        *   Create integration tests to verify the interaction between services.
    *   Goal 11:  Refactor and Optimize
        *   Review code for potential improvements and refactor as needed.
        *   Optimize database queries and gRPC calls.
    *   Goal 12: Basic Deployment Concepts
        *   Explore basic deployment strategies (e.g., using Docker Hub or a cloud provider).
        *   Deploy the application to a local Kubernetes cluster (using Minikube).

## Done Looks Like
_how do I know I'm done?_

## Branches


## Prerequisites & Documentation:

*   **Go (Golang):**
    *   *Theoretical Aspect:* Understanding Go syntax, data types, control structures, concurrency, and package management.
    *   *Documentation:* Start with "A Tour of Go" and "How to Write Go Code" on the official Golang website to grasp the basics.
    *   *Installation:* Follow the official installation guide for your operating system.
*   **gRPC:**
    *   *Theoretical Aspect:* Understanding the concept of Remote Procedure Calls, Protocol Buffers, and service definitions.
    *   *Documentation:* Refer to the official gRPC documentation for Go. Focus on defining services, generating code, and implementing client-server communication.
    *   *Tools:* Install the Protocol Buffer compiler (`protoc`) and the Go gRPC plugin.
*   **GraphQL:**
    *   *Theoretical Aspect:* Grasp the fundamentals of GraphQL queries, mutations, and schemas.  Understand how GraphQL acts as an API layer.
    *   *Documentation:* Explore the official GraphQL documentation.  Pay close attention to defining schemas, resolvers, and integrating with Go.
    *   *Libraries:*  gqlgen is used in the sample project to generate GraphQL files[1].
*   **Docker:**
    *   *Theoretical Aspect:* Learn about containerization, Docker images, Dockerfiles, and Docker Compose.
    *   *Documentation:*  Start with the official Docker documentation.  Focus on building images, running containers, and managing multi-container applications with Docker Compose.
    *   *Installation:* Install Docker Desktop for your operating system.
*   **PostgreSQL:**
    *   *Theoretical Aspect:*  Understand relational databases, SQL, and database design principles.
    *   *Documentation:* Refer to the PostgreSQL documentation for setup and basic SQL commands.
    *   *Installation:* Install PostgreSQL and a client tool like pgAdmin.
*   **Elasticsearch:**
    *   *Theoretical Aspect:*  Learn about NoSQL databases, indexing, and search concepts.
    *   *Documentation:*  Refer to the Elasticsearch documentation for setup and basic operations.
    *   *Installation:* Install Elasticsearch and a tool like Kibana.



## Plans
- Theoritcal Aspects:
	- [x] GO
	- [x] gRPC
	- [x] GraphQL
	- [ ] Microservices
	- [ ] PostgreSQL
	- [ ] ElasticSearch
	- [ ] Docker

## Journal
- 


## Files
```dataview
TABLE WITHOUT ID 
	link(file.name,file.aliases[0]) as "Note",
	Comments as "Description"
WHERE 
	contains(file.path, this.file.folder) 
	AND file.name != this.file.name
SORT file.aliases[0] ASC
```


## Connections
- [[2025-02-22]] - Daily Note for day this file was created.