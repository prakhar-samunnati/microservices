
# NestJS Microservices Project

This repository contains a NestJS microservices architecture with the following services:

- `user`: Handles user-related operations.
- `communication`: Manages communication between users.
- `gateway`: Acts as the API gateway to route requests to the appropriate services.

Each microservice is included in this repository as a submodule.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Clone the Repository](#clone-the-repository)
  - [Install Dependencies](#install-dependencies)
  - [Running the Services](#running-the-services)
  - [Installing Submodule Dependencies](#installing-submodule-dependencies)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

### Prerequisites

Make sure you have the following installed on your system:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [npm](https://www.npmjs.com/)
- [Git](https://git-scm.com/)

### Clone the Repository

To clone this repository along with its submodules, use the following command:

```bash
git clone --recurse-submodules https://github.com/your-username/your-repo-name.git
```

If you've already cloned the repository without submodules, you can initialize and update them with:

```bash
git submodule update --init --recursive
```

### Install Dependencies

Navigate to the root directory of the repository and install the dependencies:

```bash
npm install
```
This will install `concurrently` and any other dependencies required to run the services.

### Installing Submodule Dependencies

Before running each microservice, make sure to install its dependencies. Navigate to each submodule directory and run:

```bash
cd user
npm install
cd ../communication
npm install
cd ../gateway
npm install
```


### Running the Services

You can start all the services simultaneously using the following command:

```bash
npm run start:all
```

This command will run the `user`, `communication`, and `gateway` services concurrently.



This will ensure that all dependencies for each microservice are installed properly.

## Project Structure

The repository is structured as follows:

```
microservices/
├── user/              # User service
├── communication/     # Communication service
├── gateway/           # Gateway service
├── package.json       # NPM scripts and dependencies
└── README.md          # This README file
```

Each service is a Git submodule and has its own directory.


This README provides comprehensive instructions for getting started with the project, including cloning the repository with submodules, installing dependencies, running the services, and contributing to the project. It also includes a section on installing submodule dependencies, which ensures that all required dependencies for each microservice are properly installed.
