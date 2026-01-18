🚀 Personal Performance OS

A production-grade distributed system to track fitness progress, gaming stats, and reading history. Built with a Microservices architecture to demonstrate backend scalability and DevOps principles.
🏗️ System Architecture

The system is composed of decoupled services communicating via an asynchronous task queue:

    API Service: Node.js/Express server that validates incoming hobby data.

    Task Queue: Redis-backed message broker (using BullMQ).

    Worker Service: Background consumer that processes tasks and handles retries.

    Database: PostgreSQL for persistent, relational data storage.

🛠️ Tech Stack

    Language: Node.js (JavaScript/TypeScript)

    API Framework: Express

    Data Store: PostgreSQL

    Queue/Cache: Redis

    Infrastructure: Docker & Docker Compose

🚥 Getting Started
Prerequisites

    Docker & Docker Compose

    Node.js (v18+)

Installation

    Clone the repository:
    Bash

    git clone https://github.com/your-username/personal-performance-os.git

    Create a .env file in the root directory (see .env.example).

    Spin up the infrastructure:
    Bash

    docker-compose up --build
