# Avago Development Environment

### Note: This project requires the following installations:

- **Docker**: Download and install Docker for your operating system. You can get it from the [Docker official site](https://www.docker.com/products/docker-desktop).
- **Docker Extension for VS Code**: Install the Docker extension in Visual Studio Code for easier container management. You can find it in the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker).

## Setup Steps

1. **Open Ubuntu Terminal**

    Open the terminal on your Ubuntu machine or any terminal that supports Linux commands.

2. **Create a New Directory**

    Use the following command to create an arbitrary folder where the project will be cloned:

    ```bash
    mkdir avago-development
    cd avago-development
    ```

3. **Clone the Projects**

    Inside this directory, clone both the **Avago Frontend** and **Avago Backend** repositories:

    - For **Avago Frontend**:

      ```bash
      git clone https://github.com/your-repo/avago-frontend.git
      ```

    - For **Avago Backend**:

      ```bash
      git clone https://github.com/your-repo/avago-backend.git
      ```

4. **Run the Docker Compose Command**

    After cloning the repositories, run the following command to start the Avago frontend container using the Docker Compose file:

    ```bash
    docker-compose -f avago.yml up
    ```

    This command will build and start the container specified in the `avago.yml` file.

5. **Open VS Code and Access Docker Extension**

    After the container is up and running:

    - Open **VS Code**.
    - Navigate to the **Docker extension** section on the left side (you should see a Docker icon).
    - In the **Containers** section, you will see a container named `avago_frontend`.

6. **Connect to the Container**

    Right-click on the `avago_frontend` container and select **Attach Shell**. This will allow you to connect directly to the running container, giving you access to the development environment inside the container.
