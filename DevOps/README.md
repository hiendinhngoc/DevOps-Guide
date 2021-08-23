## DevOps Guide Topic Wise:

### 1. Programming Language

- Python : Scripting for web 
- Shell  : Scripting for servers 
- Yml    : For Configuration of Cloud files
- Golang : Servers and Cloud Architectures
- Javascript : Good to know for any web-development works
-  Markdown : For documentation 


### 2. OS-Concepts

- [Overview(optional)](#overview)
- Process Management
- Threads and Concurrency
- Sockets
- POSIX Basics
- Networking concepts
- Cron Jobs
- I/O Management
- Vitualization
- Memory Processes and Management
- File Systems
- Scheduling

### 3. Maintaining Servers
- Networking Concepts
- Security Concepts - OWASP-Top 10
- Protocols
- Reverse Proxy | Proxy | Forward Proxy
- Caching Servers
- Load Balancer
- Firewall
- Webservers
  - Python : WSGI | uWSGI | Tornado
  - Nginx
  - Apache
  - Caddy
  - IIS
  - Tomcat
  - Node.js


### 4. Terminal Commands

- Text Manipulation
- Process Monitoring
- Networking Processes
- Bash scripting
- Performance Management
- vim
- AWS CLI
- Kubernetes CLI
- Docker CLI
- Cloud CLIs

### 5. Infrastructure as Code

- CI/CD
  - Travis CI
  - Circle CI
  - Gitlab
  - Jenkins
  - Azure 

- Configuration Management
    - Ansible
    - Chef
    - Puppet
    - salt

- Containers
  - Docker
  - LXC

- Container Orchestration
  - Kubernetes
  - Mesos
  - Docker SWARM
  - Nomad
  - Minikube
  - Openshift
  - Amazon ECS
  - Google Kuberenetes Engine (GKE)

- Infrsatructure Provisioning
  - Hashicorp Terraform
  - AWS Cloudformation
  - Pulmi
  - Redhat Ansible
  - Azure Automation

### 7. Infrastructure Monitoring

- Prometheus
- Grafana
- Nagios
- Zabbix

### 6. Application Monitoring

- Jaegar 
- New Relic 
- Open Tracing
- Traceview

### 8. Cloud Providers

- Amazon AWS
- Google GCP
- Microsoft Azure
- Digital Ocean
- Linode
- Vultr

### 9. Log Management

- Elastic Stack
- Graylog
- Splunk
- Papertrail

### 10. Version Control

- Github
- Bitbucket
- Mercurial 

***************
### 1. Programming Language


### 2. OS-Concepts

  #### Overview
  - **OS services**
      - User interfaces: GUI, touch screen, command line
      - Program execution: load program in to memory, run and end this program.
      - I/O operations: involves file or I/O device.
      - File system manipulation: read and write files and directories, create and delete them by name, search, list info. Also include permission management.
      - Communication: occurs between processes that are executing on the same computer or different computer systems tied together by a network. Be implemented via shared memory or message passing.
      - Error detection: The OS need to be detecting and correcting errors constantly, should take appropriate action to ensure correct and consistent computing.
      - Resource allocation: allocates resources for all of the running processes.
      - Logging: keeps track of which programs use how much and what kinds of computer resources. Use for accounting or accumulating usage statistics.
      - Protection and security: ensures all access to system resources is controlled. requires authentication to the system.
  - **User and OS interface**
      - Command line: the main function is to get and execute the next user-specified command. There are two way to implement commands: cli contains the code to execute the command or cli search and load file name identical with command to memory and execute it with parameter, all logic of the command is in the file.
      - GUI: Users employ a mouse-based window and menu system characterized by a desktop metaphor.
      - Touch screen:
  - **System calls**
      - Application programming interface: typically, application developers design programs according to an application programming interface(API). The API specifies a set of functions that are passed to each function and the return values the programmer can expect. Three of the most common APIs avable to application programmers are Windows API for Windows system, the POSIX API for POSIX-based system(including virtually all versions of UNIX, Linux, and maxOS), and the Java API for programs that run on the Java virtual machine.
      - Types of system calls: 6 major types
          - Process control
          ◦ create process, terminate process
          ◦ load, execute
          ◦ get process attributes, set process attributes
          ◦ wait event, signal event
          ◦ allocate and free memory
          - File management
          ◦ create file, delete file
          ◦ open, close
          ◦ read, write, reposition
          ◦ get file attributes, set file attributes
          - Device management
          ◦ request device, release device
          ◦ read, write, reposition
          ◦ get device attributes, set device attributes
          ◦ logically attach or detach devices
          - Information maintenance
          ◦ get time or date, set time or date
          ◦ get system data, set system data
          ◦ get process, file, or device attributes
          ◦ set process, file, or device attributes
          - Communications
          ◦ create, delete communication connection
          ◦ send, receive messages
          ◦ transfer status information
          ◦ attach or detach remote devices
          - Protection
          ◦ get file permissions
          ◦ set file permissions
  - **System Services**

      Also known as system utilities,provide a convenient environment for program development and execution.

      Categories:

      - File management. These programs create, delete, copy, rename, print, list, and generally access and manipulate files and directories.
      - Status information. Some programs simply ask the system for the date, time, amount of available memory or disk space, number of users, or similar status information. Others are more complex, providing detailed performance, logging, and debugging information. Typically, these pro-grams format and print the output to the terminal or other output devices or files or display it in a window of the GUI . Some systems also support a registry, which is used to store and retrieve configuration information.
      - File modification. Several text editors may be available to create and modify the content of files stored on disk or other storage devices. There may also be special commands to search contents of files or perform transformations of the text.
      - Programming-language support. Compilers, assemblers, debuggers, and interpreters for common programming languages (such as C, C++, Java, and Python) are often provided with the operating system or available as a separate download.
      - Program loading and execution. Once a program is assembled or compiled, it must be loaded into memory to be executed. The system may provide absolute loaders, relocatable loaders, linkage editors, and overlay loaders. Debugging systems for either higher-level languages or machine language are needed as well.
      - Communications. These programs provide the mechanism for creating virtual connections among processes, users, and computer systems. They allow users to send messages to one another’s screens, to browse web pages, to send e-mail messages, to log in remotely, or to transfer files from one machine to another.
      - Background services. All general-purpose systems have methods for launching certain system-program processes at boot time. Some of these processes terminate after completing their tasks, while others continue to run until the system halted.
  - **Linkers and loaders**
      - Source files are compiled into object files that are designed to be loaded into any physical memory location, a format known as a relocatable object file.
      - Linker combines relocatable object files into a single binary executable file.
      - Loader is used to load the binary executable file into memory, where it is eligible to run on the CPU core.
