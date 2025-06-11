Here are **40 essential Docker interview questions with concise, accurate answers**, spanning basic, intermediate, and advanced levels. 🚢

---

### 🔹 **Basic Docker Questions (1–13)**

1. **What is Docker?**
   Docker is an open-source platform that automates building, shipping, and running applications in lightweight, portable containers ([vskills.in][1]).

2. **What is a Docker container?**
   A running instance of a Docker image—isolated, lightweight, and self-contained ([turing.com][2]).

3. **How does Docker differ from VMs?**
   Containers share the host OS kernel and are more lightweight and faster to start than full-fledged VMs ([vskills.in][1]).

4. **What is a Docker image?**
   A read-only template containing application code, libraries, and dependencies, used to launch containers ([turing.com][2], [vskills.in][1]).

5. **Difference between image and container?**
   Image = blueprint; Container = live running instance of that blueprint ([vskills.in][1]).

6. **What is Docker Hub?**
   A cloud-based registry for storing and distributing Docker images ([vskills.in][1]).

7. **How to check installed Docker version?**
   Run `docker --version` or `docker version`.

8. **What is a Dockerfile?**
   A script with instructions to build a Docker image ([vskills.in][1]).

9. **Basic Docker commands:**
   `docker run`, `docker ps`, `docker exec`, `docker stop`, `docker build` ([en.wikipedia.org][3], [geeksforgeeks.org][4]).

10. **What is Docker Compose?**
    Tool for defining and running multi-container apps via a YAML file (docker-compose.yml) ([vskills.in][1], [en.wikipedia.org][3]).

11. **Where are Docker volumes stored?**
    On the host at `/var/lib/docker/volumes` ([geeksforgeeks.org][4]).

12. **Who created Docker?**
    Originally authored by Solomon Hykes, written in Go ([mygreatlearning.com][5]).

13. **Why use Docker?**
    Portability, consistency, isolation, efficiency, and support for microservices ([razorops.com][6]).

---

### 🔹 **Intermediate Docker Questions (14–27)**

14. **Difference between CMD and ENTRYPOINT?**

    * `CMD`: default arguments; overridable.
    * `ENTRYPOINT`: main executable; more rigid ([geeksforgeeks.org][4], [reddit.com][7]).

15. **Difference between daemon-level and container-level logging?**

    * Daemon logs apply globally; container logs via `docker logs <id>` ([geeksforgeeks.org][4]).

16. **What does `docker info` do?**
    Shows detailed Docker environment info — containers, images, drivers ([geeksforgeeks.org][4]).

17. **Difference between image and layer?**
    Images comprise multiple layers, enabling reuse and caching ([reddit.com][8], [geeksforgeeks.org][4]).

18. **Restart policies (`no`, `on-failure`, `always`)?**
    Controls container auto-restart behavior ([geeksforgeeks.org][4]).

19. **Docker volume management?**
    Use `docker volume create|ls|inspect|rm` and mount with `-v` ([geeksforgeeks.org][4], [coreskills.interviewgemini.com][9]).

20. **Docker network types?**
    Bridge, Host, Overlay (Swarm), MacVLAN, None ([coreskills.interviewgemini.com][9]).

21. **Difference between bridge and host networking?**

    * Bridge: isolated network
    * Host: shares host’s network namespace ([sevenmentor.com][10]).

22. **What is Docker Swarm?**
    Native clustering/orchestration solution with built-in load balancing ([geeksforgeeks.org][4]).

23. **How to scale containers horizontally?**
    E.g., using `docker-compose up --scale web=3` or Swarm replication ([geeksforgeeks.org][4]).

24. **What are Docker secrets?**
    Secure management of sensitive data, encrypted and accessible only to authorized containers ([preethi-devops.com][11]).

25. **What are container registry functions?**
    Central storage & versioning for Docker images (e.g., Docker Hub, ECR) ([preethi-devops.com][11], [datacamp.com][12]).

26. **Multi-stage builds?**
    Use multiple `FROM` stages to optimize image size and discard build-only layers ([sevenmentor.com][10]).

27. **Docker container lifecycle stages?**
    Create → Run → Pause → Stop → Delete ([datacamp.com][12]).

---

### 🔹 **Advanced Docker Questions (28–40)**

28. **Image caching during builds?**
    Docker caches each layer; unchanged instructions reuse cache for faster builds ([reddit.com][8]).

29. **Optimizing image size?**
    Multi-stage builds, fewer layers, smaller base images (like Alpine), cleaning up artifacts ([testgorilla.com][13]).

30. **Dangling images?**
    Un-tagged images; removed via `docker image prune -f` ([datacamp.com][12]).

31. **Inspect image metadata?**
    Use `docker inspect <image>` to view configuration, labels, layers .

32. **Limiting CPU/Memory?**
    Use `--cpus` and `-m` flags with `docker run` ([sevenmentor.com][10], [geeksforgeeks.org][4]).

33. **Data persistence strategies?**
    Use Docker volumes, bind mounts, or external storage ([sevenmentor.com][10]).

34. **SecComp and resource limiting?**
    Use seccomp profiles and `--cpus/--memory` to restrict container capabilities and resource usage ([datacamp.com][12]).

35. **Container isolation?**
    Uses Linux namespaces and cgroups for process, network, and resource isolation .

36. **Docker content trust?**
    Enables image signing and signature validation for security ([preethi-devops.com][11], [geeksforgeeks.org][4]).

37. **Securing inter-container communication?**
    Use TLS/HTTPS, network segmentation, and Docker secrets ([preethi-devops.com][11]).

38. **Zero-downtime deployment strategies?**
    Use rolling updates (Swarm/K8s) or blue-green deployments by switching traffic ([preethi-devops.com][11]).

39. **Docker orchestration role?**
    Manages multi-container deployments, scaling, service discovery, and load balancing ([preethi-devops.com][11]).

40. **Security best practices?**
    Use minimal base images, seccomp, mount secrets appropriately, scan images, and monitor runtime .

---

These questions will give you strong preparation for Docker interviews. If you'd like, I can provide:

* Dockerfile examples
* Multi-stage build demos
* Docker Compose and Swarm orchestration examples
* Security best-practice checklists

