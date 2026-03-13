Run the Project Using Docker
Follow the steps below to run this Django project using Docker.
1. Clone the Repository
    git clone <repository-url>
    cd <project-folder>

2. Build the Docker Image
Run the following command to build the Docker image:
    docker build -t <image-name> .

This command will create a Docker image for the project using the Dockerfile.
3. Run the Application Using Docker Compose
Start the container with:

    docker-compose up
    or (new Docker versions)
    docker compose up

This will:
Start the container
Run the Django development server
Map the container port to your local machine

4. Access the Application
Once the container starts, open your browser and visit:
http://127.0.0.1:8000

5. Live Code Changes
The project uses Docker volumes, which means:
Your local project files are linked to the container files
Any change you make in the local code will automatically reflect inside the container
So you do not need to rebuild the container every time you modify the code.