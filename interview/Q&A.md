
________________________________________
1. Linux File System Hierarchy - 19 Directories
Q: What are the main directories in the Linux file system hierarchy?
A:
1.	/ – Root directory
2.	/bin – Essential binary executables
3.	/boot – Bootloader files
4.	/dev – Device files
5.	/etc – Configuration files
6.	/home – User home directories
7.	/lib – Shared libraries
8.	/media – Removable media
9.	/mnt – Mount point
10.	/opt – Optional software
11.	/proc – Process information
12.	/root – Root user home
13.	/run – Runtime data
14.	/sbin – System binaries
15.	/srv – Service data
16.	/sys – System information
17.	/tmp – Temporary files
18.	/usr – User programs
19.	/var – Variable data (logs, spool, etc.)
________________________________________
2. File System Type
Q: What are common Linux file system types?
A: ext3, ext4, xfs, btrfs, FAT32, NTFS (read-only support), and swap.
________________________________________
3. Shell and Its Types
Q: What is a shell and what are its types?
A: A shell is a command-line interface to interact with the OS. Types include:
•	Bash (Bourne Again Shell)
•	sh (Bourne Shell)
•	csh (C Shell)
•	ksh (Korn Shell)
•	zsh (Z Shell)
________________________________________
4. Kernel and Its Types
Q: What is a kernel and what are its types?
A: The kernel is the core of the OS managing hardware and system processes. Types:
•	Monolithic Kernel
•	Microkernel
•	Hybrid Kernel
•	Exokernel
________________________________________
5. Redirection in Linux
Q: What is redirection in Linux?
A: Redirecting input/output using operators:
•	> Output redirection
•	>> Append
•	< Input redirection
•	2> Error redirection
________________________________________
6. Check CPU Container Utilization
Q: How to check CPU usage of a container?
A:
docker stats <container_id>
________________________________________
7. Permission Types in Linux
Q: What are permission types in Linux?
A: Read (r), write (w), and execute (x) for user, group, and others.
________________________________________
8. What is CIDR
Q: What is CIDR?
A: Classless Inter-Domain Routing – a method for IP address allocation and routing, e.g., 192.168.0.0/24.
________________________________________
9. Network Classes
Q: What are network classes?
A:
•	Class A: 1.0.0.0 to 126.0.0.0
•	Class B: 128.0.0.0 to 191.255.0.0
•	Class C: 192.0.0.0 to 223.255.255.0
•	Class D: Multicast
•	Class E: Reserved
________________________________________
10. Public vs Private IP
Q: What is the difference between public and private IP?
A:
•	Public IP: Routable on the internet.
•	Private IP: Used within local networks (e.g., 192.168.x.x).
________________________________________
11. What is a Key and Its Types
Q: What is a key in context of SSH and its types?
A: SSH keys authenticate users. Types:
•	Private Key
•	Public Key
•	Formats: RSA, DSA, ECDSA, Ed25519
________________________________________
12. SSH Configuration File
Q: What is the SSH config file path?
A:
•	Client config: ~/.ssh/config
•	Server config: /etc/ssh/sshd_config
________________________________________
13. How Many Servers in Linux Created
Q: How many types of servers can be created on Linux?
A: Linux can host many server types: Web (Apache, Nginx), DB (MySQL), FTP, DNS, Mail, SSH, File server, etc.
________________________________________
14. What is a Server?
Q: What is a server?
A: A server is a system that provides services or resources to other devices (clients) over a network.
________________________________________
15. Firewall in Linux
Q: What is a firewall in Linux?
A: A firewall controls incoming/outgoing network traffic. Tools: iptables, firewalld, ufw.
________________________________________
16. OSI Model
Q: What is the OSI model?
A: 7-layer network model:
1.	Physical
2.	Data Link
3.	Network
4.	Transport
5.	Session
6.	Presentation
7.	Application
________________________________________
17. Launch Template
Q: What is a launch template in AWS?
A: It's a pre-defined configuration for launching EC2 instances with AMI, instance type, key, etc.
________________________________________
18. What is a Protocol
Q: What is a protocol?
A: A set of rules for data communication. Examples: HTTP, FTP, TCP, IP.
________________________________________
19. Auto Scaling Group
Q: What is an Auto Scaling Group (ASG)?
A: A feature in AWS that automatically adjusts the number of EC2 instances based on demand.
________________________________________
20. Check Kernel Version
Q: How to check the kernel version in Linux?
A:
uname -r
________________________________________
Let me know if you'd like this in PDF or formatted notes.
Here’s the continuation of the interview Q&A from 21 to 40:
________________________________________
21. Scaling Policies
Q: What are scaling policies in AWS?
A: They define how AWS Auto Scaling should behave. Types include:
•	Target Tracking Scaling
•	Step Scaling
•	Simple Scaling
•	Scheduled Scaling
________________________________________
22. AWS CloudTrail
Q: What is AWS CloudTrail?
A: A service that records all AWS API calls for account activity auditing.
________________________________________
23. What is Maven
Q: What is Maven?
A: A build automation tool for Java projects that manages project dependencies, builds, and documentation.
________________________________________
24. POM.xml
Q: What is pom.xml and its full form?
A: Full form: Project Object Model. It defines project dependencies, build configuration, and plugins in a Maven project.
________________________________________
25. Read the pom.xml
Q: What information can you get from pom.xml?
A:
•	Project coordinates (groupId, artifactId, version)
•	Dependencies
•	Plugins
•	Build info
•	Properties
•	Repository details
________________________________________
26. Use of eksctl and kubectl
Q: What are eksctl and kubectl used for?
A:
•	eksctl: CLI to create and manage AWS EKS clusters.
•	kubectl: CLI to interact with Kubernetes clusters.
________________________________________
27. Docker Architecture
Q: Explain Docker architecture.
A:
•	Docker Client: Interface to interact with Docker
•	Docker Daemon: Manages images, containers
•	Docker Images: Read-only templates
•	Docker Containers: Running instances
•	Docker Registry: Stores images (e.g., Docker Hub)
________________________________________
28. Kubernetes (K8s) Architecture
Q: Explain Kubernetes architecture.
A:
•	Master Node: API Server, Controller Manager, Scheduler, etcd
•	Worker Node: kubelet, kube-proxy, Container Runtime
•	Pods: Smallest deployable unit
________________________________________
29. Build Tool
Q: What is a build tool?
A: A tool to automate code compilation, testing, packaging, and deployment. Examples: Maven, Gradle, Ant.
________________________________________
30. Use Cases of Route 53
Q: What are the use cases of Route 53?
A:
•	Domain registration
•	DNS resolution
•	Health checking
•	Routing policies (e.g., weighted, latency-based)
________________________________________
31. AWS vs GCP
Q: Why use AWS over GCP?
A: AWS has broader services, global reach, mature ecosystem, better community support. GCP is better for AI/ML workloads.
________________________________________
32. Types of Files
Q: What are file types in Linux?
A:
•	Regular files -
•	Directory d
•	Symbolic link l
•	Character device c
•	Block device b
•	FIFO (named pipe) p
•	Socket s
________________________________________
33. What is a Subnet Mask
Q: What is a subnet mask?
A: It defines the network and host portions of an IP address. Example: 255.255.255.0
________________________________________
34. What is an Inode Number
Q: What is an inode number?
A: A unique identifier for each file containing metadata (permissions, owner, timestamps), not the file name.
________________________________________
35. Types of Users
Q: What are the types of users in Linux?
A:
•	Root User
•	System User
•	Normal User
________________________________________
36. How Many Regions in AWS
Q: How many regions are there in AWS (as of 2025)?
A: Over 32 regions globally (check AWS Regions) for latest numbers.
________________________________________
37. Skeleton File
Q: What is a skeleton file in Linux?
A: Default config files copied to a new user’s home directory from /etc/skel/.
________________________________________
38. User UID
Q: What is a user UID in Linux?
A: UID (User IDentifier) is a unique number assigned to each user. Root has UID 0.
________________________________________
39. AWS Quota (Limit)
Q: What is the quota (limit) in AWS?
A: AWS sets default service limits (e.g., EC2 instances, VPCs per region). Limits can be increased via request.
________________________________________
40. MariaDB Configuration File
Q: What is the configuration file of MariaDB?
A:
•	Main config: /etc/my.cnf or /etc/mysql/mariadb.conf.d/50-server.cnf
•	It defines ports, storage engines, buffer sizes, etc.
________________________________________
Let me know if you'd like a PDF or one-liner cheat sheet.
Here’s the final set of interview Q&A (41 to 60) for your preparation:
________________________________________
41. SSH Authentication Types
Q: What are the types of SSH authentication?
A:
•	Password-based
•	Public Key Authentication (RSA, DSA, ECDSA, Ed25519)
•	Host-based
•	GSSAPI (Kerberos)
________________________________________
42. Nginx Port Number
Q: What is the default port of Nginx?
A:
•	HTTP: 80
•	HTTPS: 443
________________________________________
43. Nginx Directory
Q: Where is the Nginx configuration directory?
A:
•	/etc/nginx/ (main config: /etc/nginx/nginx.conf)
________________________________________
44. Use Cases of SNS (Simple Notification Service)
Q: What are the use cases of AWS SNS?
A:
•	Send alerts/notifications
•	Fan-out messaging to SQS, Lambda
•	Application monitoring
•	Email/SMS/push notification delivery
________________________________________
45. What is Monitoring and Its Types
Q: What is monitoring and what are its types?
A: Monitoring tracks system performance and health. Types:
•	Infrastructure monitoring (CPU, RAM)
•	Application monitoring
•	Network monitoring
•	Log monitoring
•	Security monitoring
________________________________________
46. Kubernetes (K8s) Objects
Q: What are Kubernetes objects?
A:
•	Pod
•	Deployment
•	ReplicaSet
•	Service
•	ConfigMap
•	Secret
•	StatefulSet
•	DaemonSet
•	Namespace
•	Job / CronJob
________________________________________
47. SDLC Model
Q: What is SDLC?
A: Software Development Life Cycle – stages in software creation:
1.	Requirement Analysis
2.	Design
3.	Development
4.	Testing
5.	Deployment
6.	Maintenance
________________________________________
48. Waterfall Model
Q: What is the waterfall model?
A: A linear SDLC model where each phase flows into the next. No iteration is allowed.
________________________________________
49. Why Use Linux?
Q: Why use Linux?
A:
•	Open-source and free
•	Stable and secure
•	Highly customizable
•	Preferred for servers, DevOps, and cloud environments
________________________________________
50. Hypervisors and Types
Q: What is a hypervisor and its types?
A: Software that creates and runs virtual machines (VMs). Types:
•	Type 1 (bare-metal): ESXi, Hyper-V, Xen
•	Type 2 (hosted): VirtualBox, VMware Workstation
________________________________________
51. Cloud Service Models
Q: What are the service models in cloud computing?
A:
•	IaaS: Infrastructure as a Service (e.g., EC2)
•	PaaS: Platform as a Service (e.g., Elastic Beanstalk)
•	SaaS: Software as a Service (e.g., Gmail, Office 365)
________________________________________
52. Dockerfile
Q: What is a Dockerfile?
A: A script containing instructions to build a Docker image (e.g., FROM, RUN, COPY, etc.)
________________________________________
53. RUN vs CMD in Dockerfile
Q: What is the difference between RUN and CMD?
A:
•	RUN: Executes during image build (e.g., installing packages)
•	CMD: Defines default command at container runtime
________________________________________
54. ENTRYPOINT in Docker
Q: What is ENTRYPOINT in Docker?
A: Defines a fixed executable that runs every time a container starts. Often used with CMD.
________________________________________
55. Endpoint
Q: What is an endpoint?
A: A network address (URL or IP + port) used to access a service, API, or application.
________________________________________
56. Compressor vs Archive
Q: What’s the difference between compression and archiving?
A:
•	Compression reduces file size (e.g., gzip, bzip2)
•	Archiving combines files (e.g., tar).
You can archive without compressing.
________________________________________
57. What is AMI
Q: What is an AMI?
A: Amazon Machine Image – a pre-configured template to launch EC2 instances, including OS, software, and settings.
________________________________________
58. Virtualization and Tools
Q: What is virtualization and which tools are used?
A: Creating virtual versions of hardware or OS. Tools: VMware, VirtualBox, KVM, Xen, Hyper-V.
________________________________________
59. Kubernetes Resources
Q: What are Kubernetes resources?
A: Objects managed via the API server. Examples:
•	Pods
•	Deployments
•	Services
•	Volumes
•	Nodes
•	ConfigMaps
•	Secrets
________________________________________
60. Hard Link vs Soft Link
Q: What’s the difference between hard and soft links?
A:
•	Hard Link: Points to inode. Still accessible even if the original is deleted.
•	Soft Link (Symbolic): Points to the file name/path. Breaks if the original file is deleted.
________________________________________

### 1. **Cluster Creation and Its Types**  
**Q:** How is a cluster created and what are its types?  
**A:**  
- A **cluster** is a group of servers (nodes) that work together.  
- **Creation tools**: `kubeadm`, `eksctl` (for AWS), `minikube`, `kops`  
- **Types**:  
  - **High-Availability Cluster**  
  - **Load Balancer Cluster**  
  - **Kubernetes Cluster**  
  - **Hadoop Cluster**  
  - **Database Cluster**

### 2. **Status Codes**  
**Q:** What are HTTP status codes?  
**A:**  
- **1xx** – Informational  
- **2xx** – Success (200 OK, 201 Created)  
- **3xx** – Redirection (301 Moved, 302 Found)  
- **4xx** – Client Error (404 Not Found, 403 Forbidden)  
- **5xx** – Server Error (500 Internal, 502 Bad Gateway)

### 3. **EBS gp2 vs gp3**  
**Q:** What is the difference between EBS `gp2` and `gp3`?  
**A:**  
| Feature      | gp2                | gp3                  |
|--------------|--------------------|-----------------------|
| IOPS         | Based on size (max 16,000) | Independent of size (up to 16,000) |
| Throughput   | Up to 250 MB/s     | Up to 1,000 MB/s     |
| Cost         | More expensive     | 20% cheaper approx.  |
| Flexibility  | Less flexible      | Highly tunable       |

### 4. **Why Software Issues Occur**  
**Q:** Why do software issues occur?  
**A:**  
- Bugs in code  
- Incompatible dependencies  
- Incorrect configurations  
- Resource limitations  
- Improper deployment  
- Network or system failures

---

### 5. **Kernel Panic**  
**Q:** What is a kernel panic?  
**A:** A critical system error where the Linux kernel can’t safely recover. Causes:  
- Corrupt hardware  
- Bad drivers  
- File system issues  
- Memory errors

---

### 6. **Linux Package Management**  
**Q:** What is Linux package management?  
**A:**  
- It refers to installing, upgrading, configuring, and removing software.  
- Package managers: `apt`, `yum`, `dnf`, `zypper`, `pacman`

---

### 7. **YUM & APT vs DPKG**  
**Q:** Difference between YUM, APT, and DPKG?  
**A:**  
- **YUM (RedHat/CentOS)**: Resolves dependencies from repos  
- **APT (Debian/Ubuntu)**: Like YUM for .deb packages  
- **DPKG**: Low-level Debian package tool (doesn’t auto-resolve dependencies)

---

### 8. **What Changes After Creating a User**  
**Q:** What happens after creating a new user in Linux?  
**A:**  
- New entry in `/etc/passwd`, `/etc/shadow`, `/etc/group`  
- Home directory created (`/home/username`)  
- Default files copied from `/etc/skel/`  
- UID and GID assigned

---

### 9. **Intra-pod vs Inter-pod Communication**  
**Q:** Difference between intra-pod and inter-pod communication in K8s?  
**A:**  
- **Intra-pod**: Communication between containers inside the same pod (via `localhost`)  
- **Inter-pod**: Communication between pods using service names or IPs (through K8s networking)

---

### 10. **Docker Network**  
**Q:** Explain Docker networking types.  
**A:**  
- **bridge**: Default for containers on a single host  
- **host**: Shares host network  
- **none**: No network  
- **overlay**: Multi-host networking (used in Docker Swarm)  
- **macvlan**: Assign MAC addresses to containers

---

### 11. **Difference Between PVC and PV in K8s**  
**Q:** What is the difference between PV and PVC?  
**A:**  
- **PV (PersistentVolume)**: Cluster resource representing storage  
- **PVC (PersistentVolumeClaim)**: User’s request for storage  
- PVC binds to PV based on size, access mode

---

### 12. **Pod YAML File**  
**Q:** What is a Pod YAML file in Kubernetes?  
**A:** A definition file used to deploy a pod. Example:
```yaml
apiVersion: v1
kind: Pod
metadata:
  name: mypod
spec:
  containers:
  - name: nginx
    image: nginx
```

---

### 13. **Docker Swarm vs Kubernetes**  
**Q:** What is the difference between Docker Swarm and Kubernetes?  
**A:**  
| Feature          | Docker Swarm         | Kubernetes           |
|------------------|----------------------|----------------------|
| Setup            | Simpler              | Complex              |
| Auto-scaling     | Manual               | Supported            |
| GUI              | Limited (Docker UIs) | Rich Dashboard       |
| Networking       | Simpler              | Advanced             |
| Community        | Smaller              | Large                |

________________________________________
14. What is Docker Compose Used For?
Q: What is Docker Compose used for?
A:
Docker Compose is used to define and manage multi-container Docker applications using a single YAML file (docker-compose.yml). It allows you to:
•	Run multiple services together (e.g., app + DB)
•	Define networks and volumes
•	Automate the build, up, and down of containers
________________________________________
15. Dockerfile vs Docker Compose File Type
Q: What are the file types of Dockerfile and Docker Compose?
A:
•	Dockerfile: Text file with .Dockerfile or no extension. Defines image build steps (e.g., FROM, RUN).
•	Docker Compose File: YAML file (docker-compose.yml) used to define and manage services, volumes, networks.
________________________________________
16. Explain CI/CD Pipeline
Q: What is a CI/CD pipeline?
A:
A CI/CD (Continuous Integration/Continuous Delivery) pipeline automates the software delivery process:
•	CI: Automates testing, building, and merging code
•	CD: Automates deployment to staging/production
Tools: Jenkins, GitHub Actions, GitLab CI, CircleCI
________________________________________
17. What is the /90s Directory in Linux?
Q: What is the /etc/sysctl.d/90-override.conf (or similar 90s) directory in Linux?
A:
It refers to override configuration files often found in /etc/sysctl.d/ or /etc/systemd/system/.
Files prefixed with 90- have a lower priority than 99- but override lower-numbered files.
This follows systemd's override mechanism based on file name order.
________________________________________
18. Skeleton File and Its Types
Q: What is a skeleton file in Linux?
A:
Skeleton files are default files copied to a new user’s home directory when created.
Location: /etc/skel/
Examples:
•	.bashrc
•	.profile
•	.bash_logout
________________________________________
19. Creating a Hidden File in Linux
Q: How to create a hidden file in Linux?
A:
Prefix the filename with a dot .:
touch .hiddenfile
Hidden files are not shown with ls unless using ls -a.
________________________________________
20. Use Cases of /etc/passwd and Explain 7 Fields
Q: What are the use cases of /etc/passwd, and what do its 7 fields mean?
A:
•	Stores user account information
•	Readable by all users
7 fields (colon : separated):
username:password:UID:GID:comment:home:shell
•	username: Login name
•	password: x refers to /etc/shadow
•	UID: User ID
•	GID: Group ID
•	comment: User's full name or description
•	home: Home directory path
•	shell: Default shell (e.g., /bin/bash)
________________________________________
21. Difference Between Rules and Policies
Q: What is the difference between rules and policies?
A:
•	Rules: Specific instructions (e.g., block port 22)
•	Policies: Higher-level decisions or strategies (e.g., deny all by default, allow specific traffic)
In firewalls:
•	Rules enforce policies.
•	Policies are sets of rules.
________________________________________
22. Load Balancer and Its Types
Q: What is a Load Balancer and its types?
A:
A Load Balancer distributes incoming network traffic across multiple servers.
Types:
•	Application (Layer 7) – HTTP/HTTPS (e.g., AWS ALB)
•	Network (Layer 4) – TCP/UDP (e.g., AWS NLB)
•	Classic Load Balancer (ELB) – Legacy (Layer 4 & 7)
________________________________________
23. NAT Gateway vs NAT Instance
Q: Difference between NAT Gateway and NAT Instance?
Feature	NAT Gateway	NAT Instance
Managed	Fully managed by AWS	User-managed EC2
Performance	Scalable automatically	Limited to instance size
Availability	High availability	Requires manual setup
Cost	More expensive	Cheaper (for low traffic)
Use Case	Production preferred	Custom configurations
________________________________________

### 24. **Explain Docker Volume**  
**Q:** What is a Docker Volume?  
**A:**  
Docker volumes are **persistent storage** used to save data outside of containers so it’s not lost after a restart.  
- Stored in `/var/lib/docker/volumes/`  
- Created using `docker volume create`  
- Mounted with `-v volume_name:/container/path`  

---

### 25. **ReplicaSet vs ReplicationController vs Deployment (K8s)**  
| Feature               | ReplicaSet            | ReplicationController   | Deployment                |
|-----------------------|------------------------|--------------------------|---------------------------|
| Purpose               | Maintains replicas     | Legacy replica manager   | Manages ReplicaSets       |
| Usage                 | Modern K8s             | Deprecated                | Recommended               |
| Rolling updates       | No                     | No                       | Yes                       |
| Rollback support      | No                     | No                       | Yes                       |

---

### 26. **Explain Block Type**  
**Q:** What is block storage?  
**A:**  
Block storage (e.g., AWS EBS) stores data in **fixed-size blocks**.  
- Used in VMs, databases  
- High performance  
- Unlike object storage (e.g., S3) or file storage

---

### 27. **Datadog Integration with EKS**  
**Q:** How to integrate Datadog with EKS?  
**A:**  
- Install the **Datadog Agent** via Helm or YAML  
- Provide API key:  
```bash
helm install datadog-agent datadog/datadog \
  --set datadog.apiKey=<DATADOG_API_KEY> \
  --set datadog.site='datadoghq.com'
```  
- Monitor metrics, logs, and traces via Datadog UI

---

### 28. **Home Directory of Tomcat Cluster**  
**Q:** What is the home directory of Apache Tomcat?  
**A:**  
Typically:  
```bash
/opt/tomcat
/usr/share/tomcat
```
In cluster setups, each node runs a Tomcat instance with its own `conf`, `webapps`, `logs`.

---

### 29. **Start Angular Server**  
**Q:** Which command starts an Angular dev server?  
**A:**  
```bash
ng serve
```
Or with port:  
```bash
ng serve --port 4201
```

---

### 30. **Change Nginx Port 80 to 81**  
**Q:** How to change Nginx port 80 to 81?  
**A:**  
Edit `/etc/nginx/sites-available/default` or `/etc/nginx/nginx.conf`:  
```nginx
server {
    listen 81;
    ...
}
```
Then reload Nginx:  
```bash
sudo systemctl reload nginx
```

---

### 31. **Nginx Proxy Server Attack**  
**Q:** What are common proxy server attacks on Nginx?  
**A:**  
- **HTTP smuggling**  
- **Request flooding (DDoS)**  
- **Open proxy abuse**  
- **Header injection**  
Mitigation: Rate limiting, header sanitization, firewall rules.

---

### 32. **Remote Proxy Setup**  
**Q:** What is a remote proxy setup?  
**A:**  
A remote proxy forwards client requests to servers across the internet.  
E.g., Nginx configured as reverse proxy to a remote backend:  
```nginx
location / {
    proxy_pass http://remote_server_ip:port;
}
```

---

### 33. **What is Bastion Host?**  
**Q:** What is a Bastion Host?  
**A:**  
A **bastion host** is a **jump server** that acts as a secure bridge to access instances in private subnets.  
- Public IP + strict firewall rules  
- Allows SSH into internal systems

---

### 34. **Instance Type – General Purpose Family in AWS**  
**Q:** What are General Purpose instance types in AWS?  
**A:**  
- Balanced CPU/RAM  
- Suitable for dev, testing, web servers  
- Examples: `t3`, `t3a`, `t4g`, `m5`, `m6i`

---

### 35. **Kubernetes Version**  
**Q:** How to check Kubernetes version?  
**A:**  
```bash
kubectl version --short
```

---

### 36. **Instance Limit Quota (AWS)**  
**Q:** What is instance limit quota in AWS?  
**A:**  
AWS limits how many EC2 instances, EBS volumes, etc., you can launch per region.  
Check via:  
- **Service Quotas console**  
- CLI:  
```bash
aws service-quotas get-service-quota --service-code ec2 ...
```

---

### 37. **OSI Model**  
**Q:** Explain OSI model layers.  
**A:**  
1. **Physical** – Hardware transmission  
2. **Data Link** – MAC, switches  
3. **Network** – IP, routers  
4. **Transport** – TCP/UDP  
5. **Session** – Connections/sessions  
6. **Presentation** – Format, encryption  
7. **Application** – User interface (HTTP, FTP)

---

### 38. **LAN, MAN, WAN**  
**Q:** What is LAN, MAN, and WAN?  
**A:**  
- **LAN**: Local Area Network (home, office)  
- **MAN**: Metropolitan Area Network (city-wide)  
- **WAN**: Wide Area Network (internet, across countries)

---

### 39. **What is Used in AWS Cloud?**  
**Q:** What components are used in AWS Cloud?  
**A:**  
- **Compute**: EC2, Lambda  
- **Storage**: S3, EBS  
- **Database**: RDS, DynamoDB  
- **Networking**: VPC, ELB  
- **Security**: IAM, KMS  
- **Monitoring**: CloudWatch, CloudTrail

---

### 40. **What is Subnet and Subnet Mask?**  
**Q:** Explain subnet and subnet mask.  
**A:**  
- **Subnet**: Subdivision of a network  
- **Subnet mask**: Defines network and host bits (e.g., `255.255.255.0`)  
- CIDR: `/24` → 256 IPs


________________________________________
41. SonarQube Architecture
SonarQube comprises several components:
•	Web Server: Provides the user interface and handles HTTP requests.
•	Compute Engine: Processes code analysis reports and updates the database.
•	Database: Stores configuration, metrics, and analysis results.
•	Scanner: Analyzes source code and sends reports to the server.(SonarQube Documentation)
This modular architecture ensures scalability and efficient code quality management. (SonarQube Documentation)
________________________________________
42. What is a Bridge Network?
In Docker, a bridge network is a private internal network that allows containers to communicate with each other. Containers on the same bridge network can interact, while isolation is maintained from containers on other networks. (Docker Documentation)
________________________________________
43. Network Adapter in AWS and Linux
•	AWS: Uses Elastic Network Interfaces (ENIs), which are virtual network cards attached to instances, allowing for flexible networking configurations. 
•	Linux: Network adapters are represented as interfaces (e.g., eth0, ens33) and can be managed using tools like ifconfig or ip.(AWS Documentation)
________________________________________
44. IP Addresses for t2.medium Instance
A t2.medium instance supports up to 3 network interfaces, each capable of having multiple private IP addresses. The exact number of IPs depends on the instance's configuration and AWS limits. (AWS Documentation)
________________________________________
45. Network Classes
IPv4 addresses are divided into classes:(Meridian Outpost)
•	Class A: 1.0.0.0 to 126.255.255.255 (Large networks)
•	Class B: 128.0.0.0 to 191.255.255.255 (Medium-sized networks)
•	Class C: 192.0.0.0 to 223.255.255.255 (Small networks)
•	Class D: 224.0.0.0 to 239.255.255.255 (Multicast)
•	Class E: 240.0.0.0 to 255.255.255.255 (Experimental) 
________________________________________
46. Kubernetes Overview
Kubernetes is an open-source platform for automating deployment, scaling, and management of containerized applications. It orchestrates containers across clusters of machines, providing high availability and scalability. 
________________________________________
47. CBSE and DVCS Explained
•	CBSE (Component-Based Software Engineering): Focuses on building software systems by integrating pre-existing components.
•	DVCS (Distributed Version Control System): Allows multiple developers to work on a project simultaneously by maintaining complete code repositories locally, facilitating offline work and better collaboration. (about.gitlab.com)
________________________________________
48. Check Git Log in One Line
Use the following command to view Git logs in a single line per commit:(Git)
git log --oneline
________________________________________
49. Change a Commit
To modify the most recent commit:(Atlassian)
git commit --amend
For earlier commits, use interactive rebase:(Stack Overflow)
git rebase -i HEAD~n
Replace n with the number of commits to go back. (Atlassian)
________________________________________
50. Create a Workspace in Terraform
To create a new workspace in Terraform:(HashiCorp Developer)
terraform workspace new <workspace_name>
This allows for managing multiple environments (e.g., dev, prod) within the same configuration. 
________________________________________
51. Language Used for Terraform
Terraform uses HashiCorp Configuration Language (HCL), a domain-specific language designed for writing infrastructure as code. (HashiCorp Developer)
________________________________________
52. Argument Reference in Terraform
In Terraform, arguments are used to assign values to resource parameters. References allow for dynamic assignment using expressions, enabling modular and reusable configurations. (HashiCorp Developer, HashiCorp Developer)
________________________________________
53. Download Dependencies and Plugins in India
Maven downloads dependencies and plugins defined in the pom.xml file during the build process. Running mvn install or mvn compile will fetch the necessary artifacts from configured repositories. (Stack Overflow)
________________________________________
54. Kubernetes Origin
Kubernetes was developed by Google, inspired by their internal Borg system, and released as an open-source project in 2014. It is now maintained by the Cloud Native Computing Foundation (CNCF). (WIRED, Wikipedia)
________________________________________
55. Languages Supported by Kubernetes
Kubernetes provides client libraries for multiple programming languages, including Go, Python, Java, and JavaScript, facilitating interaction with its API. (Kubernetes)
________________________________________
56. What is a Node in Kubernetes
A node in Kubernetes is a worker machine (virtual or physical) that runs containerized applications. Each node contains the necessary services to run pods and is managed by the master components.
________________________________________
57. Node Control API Version
Kubernetes nodes communicate with the control plane using the Kubernetes API, which follows semantic versioning (e.g., v1.20). The specific API version can be checked using:
kubectl version
________________________________________
58. Communication Between Worker Node and Master Node
Worker nodes communicate with the master node through the Kubernetes API server. This communication is secured using certificates and is essential for cluster operations.
________________________________________
59. Service Types in Kubernetes
Kubernetes supports several service types:
•	ClusterIP: Accessible only within the cluster.
•	NodePort: Exposes the service on each node's IP at a static port.
•	LoadBalancer: Provisions an external load balancer (if supported).
•	ExternalName: Maps the service to the contents of the externalName field (e.g., DNS name).
________________________________________
60. Umarks Stored Path
The term "Umarks" is unclear in this context. If you meant "bookmarks," their storage path depends on the application and operating system. Please provide more details for a specific answer.
________________________________________
61. Define CI, CD, and Related Terms
•	Continuous Integration (CI): Regularly merging code changes into a shared repository, followed by automated builds and tests.
•	Continuous Deployment (CD): Automatically deploying every change that passes tests to production.
•	Continuous Delivery: Ensuring code is always in a deployable state, with deployments triggered manually.
•	Continuous Monitoring: Ongoing observation of system performance and health in real-time.
•	Version Control: Managing changes to source code over time, typically using systems like Git.
________________________________________
