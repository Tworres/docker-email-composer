# Docker Email Sender Simulation

This project utilizes Docker to create a network of interconnected servers that simulate an email sender environment. By running Docker containers, you can easily set up and manage the simulation environment for testing email sending functionality.

## Getting Started

To get started with this project, follow these steps:

1. **Install Docker**: Ensure Docker is installed on your system. You can download and install Docker from the [official website](https://www.docker.com/get-started).

2. **Clone the Repository**: Clone this repository to your local machine using the following command:
    ```
    git clone <repository-url>
    ```

3. **Build Docker Images**: Navigate to the project directory and build the Docker images using the provided Dockerfiles. Run the following command:
    ```
    docker-compose build
    ```

4. **Start Docker Containers**: Once the images are built, start the Docker containers by running:
    ```
    docker-compose up
    ```

5. **Scaling Workers (Optional)**: You can also scale the number of worker instances to improve sending time. For example, to run three instances of the worker, use the following command:
    ```
    docker-compose up --scale worker=3
    ```

6. **Access the Simulation Environment**: Once the containers are up and running, you can access the simulation environment through the configured ports. Refer to the documentation for details on accessing different components of the simulation.

## Usage

To observe the system in action, ensure that the docker-compose is running. Once it's running, navigate to localhost:8081 in your web browser. Fill in the required fields and submit the form.

Upon successful submission, you'll receive a confirmation message from the backend indicating that the message was sent successfully.

To monitor the activity of the workers, you can view their logs using the command docker-compose logs -f -t. This command provides real-time logs, allowing you to track the progress and activities of the workers.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or create a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
