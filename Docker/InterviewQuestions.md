### ✅ Docker Interview Questions and Answers

---

#### 🔹 **Common Docker Interview Questions**

**1. What is Docker, and how does it differ from traditional virtualization?**

* Docker is a containerization platform that packages applications with their dependencies into containers. Unlike traditional virtualization, which uses hypervisors to emulate hardware, Docker shares the host OS kernel, resulting in lightweight, faster, and more efficient resource usage.

**2. Explain the key components of Docker's architecture.**

* **Docker Engine**: Core client-server application
* **Docker Daemon**: Runs in the background and manages Docker objects
* **Docker Client**: CLI to interact with Docker
* **Images**: Read-only templates used to create containers
* **Containers**: Runtime instances of images
* **Docker Registries**: Stores and distributes Docker images (e.g., Docker Hub)

**3. What are Docker containers, and how do they work?**

* Docker containers are lightweight, portable, and isolated environments to run applications. They share the host OS kernel but maintain their own filesystem, network, and process space.

**4. How do you create a Docker image? Explain Dockerfile.**

* A **Dockerfile** is a script with instructions to build an image.
  Example:

```Dockerfile
FROM node:18
COPY . /app
WORKDIR /app
RUN npm install
CMD ["node", "app.js"]
```

* Use `docker build -t myimage .` to create the image.

**5. Difference between image and container in Docker?**

* **Image**: Blueprint (read-only) of an application
* **Container**: Running instance of an image

**6. What is Docker Compose?**

* Docker Compose is a tool to define and manage multi-container applications using a `docker-compose.yml` file.
* Simplifies local development and orchestration.

**7. Describe Docker networking modes.**

* **Bridge** (default): Isolated network
* **Host**: Container shares host network
* **None**: No networking
* **Overlay**: Multi-host communication (Swarm)

**8. How do you manage data persistence?**

* Use **volumes** or **bind mounts** to persist data outside containers.
* Volumes are preferred for long-term storage and backups.

**9. Explain Docker volumes.**

* Managed by Docker and stored under `/var/lib/docker/volumes`
* Use `docker volume create`, `docker run -v`, `docker-compose` to manage them
* Useful for sharing data between containers

**10. How do you secure Docker containers/images?**

* Use official base images
* Regularly scan images for vulnerabilities
* Use `USER` directive to avoid root
* Enable Docker Content Trust
* Use least privilege for container permissions

**11. What is multistage Dockerfile and how does caching work?**

* Multistage builds use multiple `FROM` statements to optimize builds.
* Reduces final image size by discarding build dependencies.
* Docker caches each layer based on changes, improving performance.

**12. Entrypoint vs CMD?**

* `CMD`: Default arguments passed to the container
* `ENTRYPOINT`: Fixed command to execute
* Combined usage: `ENTRYPOINT ["python"]`, `CMD ["app.py"]`

**13. How to optimize lightweight Docker containers?**

* Use minimal base images like Alpine
* Remove unnecessary dependencies
* Use multistage builds
* Clean up package cache after install

---

#### 🔹 **Scenario-Based Docker Interview Questions**

**1. Dockerized app uses a DB – how to manage persistence & backups?**

* Mount database data directory to a volume
* Automate daily backups using cron inside another container or via host
* Optionally sync to S3 or offsite storage

**2. Ensuring dev & prod consistency with Docker Compose?**

* Use the same `docker-compose.yml` with environment-specific override files (e.g., `docker-compose.prod.yml`)
* Store configuration in `.env` files and secrets manager

**3. Image versioning & microservices updates?**

* Tag images using semantic versioning (e.g., `v1.0.1`)
* Use CI/CD pipelines to build, test, and push images
* Maintain a registry (like ECR) and use `latest` only for dev
* Use canary or blue-green deployments for updates

**4. Memory leak in production container – what steps?**

* Monitor with tools (cAdvisor, Prometheus)
* Use `docker stats` for resource usage
* Use logging and APM tools (e.g., Datadog, New Relic)
* Check for long-running or orphan processes
* Restart with memory limits to mitigate temporarily

**5. Docker security best practices?**

* Avoid running as root
* Limit container capabilities using `--cap-drop`
* Use signed images and enforce policies with tools like Docker Bench, Clair
* Regularly update base images and use vulnerability scanners

**6. Migrating app to new host with Docker?**

* Save image with `docker save` and transfer via SCP
* Or push to Docker registry and pull on new host
* Transfer data volumes if needed
* Use `docker-compose up` to recreate

**7. Blue-Green deployment strategy with Docker?**

* Maintain two environments (blue and green)
* Deploy new version to green, test it
* Switch traffic (via DNS or load balancer)
* Keep blue for rollback

**8. Monitoring Docker containers in production?**

* Tools: Prometheus + Grafana, ELK/EFK stack, cAdvisor, CloudWatch, Datadog
* Practices:

  * `HEALTHCHECK` in Dockerfiles
  * Logging drivers (json-file, fluentd)
  * Resource limits and alerts
  * Centralized monitoring dashboards
