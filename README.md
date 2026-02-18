<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Create a Docker Container using Cursor

**Project Link:** [View Project](http://learn.nextwork.org/projects/ai-mcp-docker)

**Author:** adeel nisar  
**Email:** adeelnisar941@gmail.com

---

---

## Introducing Today's Project!

I am using Cursor’s AI to build and manage a PostgreSQL database inside a Docker container using the Model Context Protocol (MCP).

In short, we are giving Cursor the power to control Docker directly so you can spin up, check, and manage a real database using just natural language prompts instead of manual terminal commands.

### Key tools and concepts

The key tools I used include
I am now proficient in these core tools and concepts:

Model Context Protocol (MCP): I am using this as the bridge that allows Cursor's AI to control my local system tools.

Cursor: I am leveraging this AI-native editor to manage infrastructure through natural language instead of manual commands.

Docker Desktop: I am using this to run PostgreSQL in an isolated, lightweight container, keeping my host machine clean.

Containers vs. Images: I am understanding that an image is the blueprint and a container is the actual running instance of the database.

Docker Compose: I am using this to define and automate the setup of my database environment so it's repeatable.

Observability: I am monitoring database health by checking container logs directly within the chat interface.

### Challenges and wins

This project took me approximately 2 hours

### Why I did this project

I am doing this project today to learn how to bridge the gap between AI and infrastructure by using natural language to control my local developer environment.

Another MCP skill I want to learn is how to connect Cursor to PostgreSQL directly via the MCP server. This would let me:

I am looking to query, edit, and visualize my database tables through chat.

I am aiming to automate schema migrations without writing manual SQL.

I am interested in connecting to other tools like GitHub or Google Search using MCP to give my AI even more real-time context.

---

## Setting Up Cursor and Docker Desktop

In this step, I am installing these tools to build a modern development environment:

I am using Cursor because its AI can use the Model Context Protocol (MCP) to talk directly to my system's tools.

Docker Desktop will help me by running the PostgreSQL database in a lightweight, isolated container without me needing to install it manually.

![Image](http://learn.nextwork.org/warm_pink_glamorous_tiger_melon/uploads/ai-mcp-docker_8h9i0j1k)

### Why Docker containers?

I am using Docker containers because:

I am keeping my system clean by running PostgreSQL in an isolated "bubble" instead of installing it directly on my OS.

I am ensuring consistency, so the database works exactly the same way every time, regardless of my computer's settings.

Docker Desktop will help me spin up or delete the entire environment in seconds with zero manual configuration.

---

## Connecting Cursor to Docker with MCP

In this step i will: Install Python and uv, a fast Python package manager.

Enable the Docker MCP in Cursor.

Verify the Docker MCP is connected.

![Image](http://learn.nextwork.org/warm_pink_glamorous_tiger_melon/uploads/ai-mcp-docker_8g9h0i1j)

### Installing Python and uv

I am installing Python because the Docker MCP (Model Context Protocol) is built on it; it acts as the translator between Cursor and my system.

I am using uv because:

I am looking for speed—it installs the necessary MCP packages much faster than standard tools.

It will help me manage the project's dependencies in a clean, isolated way without messing up my global Python settings.

### What the Docker MCP can do

With the Docker MCP, you can perform these main actions:
List containers
See all Docker containers on your system (running, exited, created).
Inspect logs
Fetch the latest logs for a specific container to debug issues.
Create standalone containers
Start new containers from an image (optionally with a name) without writing a full docker run command.
Deploy Docker Compose stacks
Bring up multi-container apps from a provided docker-compose YAML definition.

---

## Creating My First PostgreSQL Container

In this step, I'm going to use the Docker MCP to Prompt Cursor to create a PostgreSQL container using the Docker MCP.

Verify the container is running in Docker Desktop..

![Image](http://learn.nextwork.org/warm_pink_glamorous_tiger_melon/uploads/ai-mcp-docker_7k8m9n0p)

### Verifying the container

Open the Docker Desktop application.

Click on the Containers tab in the left sidebar.

Look for container name:

A Green icon/label indicates it is "Running."

A Grey or Red icon means it is "Exited" or "Paused."

![Image](http://learn.nextwork.org/warm_pink_glamorous_tiger_melon/uploads/ai-mcp-docker_2q3r4s5t)

---

## Orchestrating Multiple Containers with Docker Compose

Create a project folder on Desktop.

Set up PostgreSQL and Adminer with Docker Compose.

Access your database in the browser.

### Setting up the docker-compose.yml file

The provided docker-compose.yml file configures two interconnected services:

PostgreSQL Database (my-db): * Runs Postgres 16-alpine.

Initializes a database named nextwork.

Sets credentials to admin / secretpass123.

Ensures the service remains active via restart: unless-stopped.

Adminer GUI (adminer):

Provides a web-based management interface.

Maps localhost:8081 to internal port 8080.

Links directly to my-db using the depends_on condition.

![Image](http://learn.nextwork.org/warm_pink_glamorous_tiger_melon/uploads/ai-mcp-docker_x7z1b4c6)

### Accessing the database in the browser

I verified my database by logging into Adminer at localhost:8080 where I can see the login page and I logged in using the docker-compose.yaml credentials.

---

## Monitoring Container Logs

In this project extension, I'm going to Use the Docker MCP to check your container's logs.

Understand what the log entries mean.

![Image](http://learn.nextwork.org/warm_pink_glamorous_tiger_melon/uploads/ai-mcp-docker_9y0z1a2b)

### What I learned from the logs

I checked my container logs by using docker mcp and giving it prompt using cursor

---

---
