# RabbitMQ POC with .NET Core

This is a proof of concept (POC) project demonstrating how to use RabbitMQ with Docker on Windows and C# with .NET Core. The project includes a simple producer that sends messages to a RabbitMQ queue and a consumer that receives and processes those messages.

## Project Structure

* Program.cs # Main entry point of the application
* Producer.cs # Contains the code for the RabbitMQ producer
* Consumer.cs # Contains the code for the RabbitMQ consumer
* RabbitMQPOC.csproj # .NET Core project file
* README.md # Project documentation


## Prerequisites

- [.NET Core SDK](https://dotnet.microsoft.com/download) (version 3.1 or later)
- [Docker Desktop](https://www.docker.com/products/docker-desktop) for Windows
- Basic knowledge of C# and RabbitMQ

## Getting Started

### 1. Set Up RabbitMQ with Docker

1. Pull the RabbitMQ Docker image:
   ```bash
   docker pull rabbitmq:3-management

2. Run the docker container
    ```bash
   docker run -d --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3-management

3. Run the project (two instances: one for producer and one for consumer)
    ```bash
    dotnet run

