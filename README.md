# CS 6888: Homework 0 - Starter Homework

## Objective

This assignment ensures you can setup your environment, execute code, and submit an assignment. It establishes the expectations for tool setup and independent problem solving.

## 1. Prerequisites

### Install Docker

You must have Docker installed to run the tool/code for this class.

1. Download **Docker Desktop** from [docker.com/get-started](https://www.docker.com/get-started).
2. After installation, verify it is working by running the following in your terminal:
```bash
docker run hello-world
```
### Get the Repository

1. Accept the assignment via the GitHub Classroom link provided on Canvas.
2. Clone the newly created private repository to your local machine.

## 2. Environment Setup

We use a pre-built Docker image to verify the environment. Execute the following commands from the root directory of the repository you just cloned:

```bash
# Pull the image and start the container
docker-compose pull
docker-compose up -d main

# Launch a shell inside the running container
docker-compose exec main bash
```

To stop the container later, run:

```bash
docker-compose stop
```

## 3. Assignment Tasks

Once you are inside the container (after running the `exec` command above), complete the following steps:

1. **Check Version:** Run `infer --version` to verify the setup.
2. **Modify Script:**
* Navigate to the homework directory: `cd files/hw0`
* Edit `run_all.sh` to include the command `infer --version`.


3. **Push Changes:** Exit the container and push your changes to GitHub.

## 4. Submission

Submit a **PDF Report** (IEEE-conference format) to Canvas under "Starter Homework". The report must include:

1. Your Computing ID.
2. Your GitHub repository address (formatted as a URL).
3. The `infer` version output (formatted as verbatim/code).
