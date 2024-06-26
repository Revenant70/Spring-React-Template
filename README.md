# Spring React Template

This is a template project for building web applications using Spring Boot for the backend and React for the frontend.

## Features

- **Spring Boot**: Backend framework for building Java-based applications.
- **React**: Frontend library for building interactive user interfaces.
- **Docker**: Containerization technology for packaging applications and dependencies.
- **Maven**: Build automation tool for managing Java projects.
- **npm**: Package manager for managing JavaScript dependencies.

## Prerequisites

Before running this project locally, ensure you have the following prerequisites installed:

- Java Development Kit (JDK)
- Node.js and npm
- Docker

## Getting Started

To get started with this template, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/Revenant70/Spring-React-Template.git
    ```

2. Navigate to the project directory:

    ```bash
    cd spring-react-template
    ```

3. change remote repo to your project:

    ```bash
    git remote set-url origin <Your new url>
    ```

5. Build the frontend:

    ```bash
    cd Frontend/
    npm install
    npm run build
    cd ..
    cd Backend/
    ```

6. Add config files to backend gitignore

    ```gitignore
    Dockerfile
    application.properties
    docker-compose.yaml
    ```

7. Build the backend:

    ```bash
    mvn package -DskipTests
    ```

8. Run the application using Docker:

    ```bash
    cd ..
    docker-compose up --build
    ```

## Development

To run the application in development mode, follow these steps:

1. Start the backend:

    ```bash
    cd Backend/
    mvn spring-boot:run
    ```

2. Start the frontend:

    ```bash
    cd Frontend/
    npm run dev
    ```

## Configuration

- Backend configuration: Modify `src/main/resources/application.properties` to configure backend properties such as database connection settings, db username, and password.
- Frontend configuration: Modify `frontend/src/config.js` to configure frontend properties such as API endpoints.

## Contributing

Contributions are welcome! Feel free to submit issues and pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
