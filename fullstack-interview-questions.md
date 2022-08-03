# Fullstack Interview Questions

## React

1. What is React and why do we use it?
    1. Library
    1. It gives us components to easily share
    1. Reusable behavior
1. What is JSX
    1. HTML & JavaScript
1. How do we pass data to React components?
    1. 2 ways: Props & Context API
1. What is the difference between State & Props
    1. States are values we can read an update in React components
    1. Props are values that are passed to React components and are read-only
1. What are react fragments used for?
    1. special feature that let you write group children elements without crating the actual node in the DOM
1. Why do we need keys for React Lists
    1. They are unique values that we must pass to the key prop when we use the .map function to loop over an element or a component
1. What is a ref? How do you use it?
    1. a ref is a reference to a DOM element in React
    2. Refs are often referred to as an "escape hatch" to be able to work with a DOM element directly. They allow us to do certain operations that can't be done through React otherwise, such as clearing or focusing an input.
1. What is the useEffect hook used for?
    1. Performing side effects in our React components. 
1. When do you use React Context vs Redux?
    1. React Context is a way to provide and consume data throughout our app without using props.   Context helps us prevent the problem of "props drilling" when passing data with props through components that don't need it.  
    1. Redux is a state library that allows us to both read and update State
1. What are the useCallback & useMemo hooks used for?

## Python

1. What is Python?
    1. high-level interpreted, general-purpose programming language with High-level data structures and dynamic typing and binding.  Python is open source.
1. What is Scope in Python?  Can you give an example of types of scope?
    1. Everyone object in python functions within a scope.  Scope is a block of code where an object in python remains relevant.
    1. Local Scope - local objects in the available in the current function
    1. global scope - objects available through the code execution
    1. module-level scope - the global objects of the current module accessible in the program
    1. outermost scope - all the built-in names callable in the program.  THe objects in this scope are searched last to find the name referenced
1. What are lists and tuples?  What is the key difference between the two?
    1. They are both sequence data types that can store a collection of objects.  The key difference between the two is lists are mutable and tuples are immutable.  
1. What are the common built-in data types in Python?
    1. NoneType
    1. numerics
        1. int, float, complex, bool
    1. Sequence types
        1. list, tuple, range, str
    1. Mapping Types
        1. dict
    1. Set Types
        1. set
        1. frozenset
1. What is pass in python?
    1. represents a null operation in python. it is generally used for the purpose of filling up empty blocks of code which may execute during runtime but has yet to be written.
1. What are global, protected and private attributes?
    1. global - public variables that are defined in the global scope.  
    1. Protected - attributes defined with an underscore prefixed to their identifier
    1. Private - double underscores, they cannot be accessed or modified from the outside directly and will result in an attribute error if an attempt is made. 
1. What is the use of self in Python?
    1. Self is used to represent the instance of the class. With this keyword, you can access the attributes and methods of the class in python. It binds the attributes with the given arguments. self is used in different places and often thought to be a keyword. But unlike in C++, self is not a keyword in Python.
1. What is docstring in Python?
    1. Documentation string or docstring is a multiline string used to document a specific code segment.
    1. The docstring should describe what the function or method does.
1. How is memory managed in Python?
    1. Memory management in Python is handled by the Python Memory Manager. The memory allocated by the manager is in form of a private heap space dedicated to Python. All Python objects are stored in this heap and being private, it is inaccessible to the programmer. Though, python does provide some core API functions to work upon the private heap space.
    2. Additionally, Python has an in-built garbage collection to recycle the unused memory for the private heap space.
1. What is pickling and unpickling?
    1. Python library offers a feature - serialization out of the box. Serializing an object refers to transforming it into a format that can be stored, so as to be able to deserialize it, later on, to obtain the original object. Here, the pickle module comes into play.




## SQL

1. What is a primary key?
    1. A primary key is a combination of fields which uniquely specify a row. This is a special kind of unique key, and it has implicit NOT NULL constraint. It means, Primary key values cannot be NULL.
2. What is a unique key?
    1. A Unique key constraint uniquely identified each record in the database. This provides uniqueness for the column or set of columns.
    1. A Primary key constraint has automatic unique constraint defined on it. But not, in the case of Unique Key.
    1. There can be many unique constraint defined per table, but only one Primary key constraint defined per table.

3. What is a foreign key?
    1. A foreign key is one table which can be related to the primary key of another table. Relationship needs to be created between two tables by referencing foreign key with the primary key of another table.

4. What is a join?
    1. This is a keyword used to query data from more tables based on the relationship between the fields of the tables. Keys play a major role when JOINs are used.
5. What are the types of join and explain each?
    1. There are various types of join which can be used to retrieve data and it depends on the relationship between tables.
    1. Inner Join.
        1. Inner join return rows when there is at least one match of rows between the tables.

6. Right Join.
    1. Right join return rows which are common between the tables and all rows of Right hand side table. Simply, it returns all the rows from the right hand side table even though there are no matches in the left hand side table.

7. Left Join.
    1. Left join return rows which are common between the tables and all rows of Left hand side table. Simply, it returns all the rows from Left hand side table even though there are no matches in the Right hand side table.

8. Full Join.
    1. Full join return rows when there are matching rows in any one of the tables. This means, it returns all the rows from the left hand side table and all the rows from the right hand side table.
1. What is normalization?
    1. Normalization is the process of minimizing redundancy and dependency by organizing fields and table of a database. The main aim of Normalization is to add, delete or modify field that can be made in a single table.
1.  What is normalization?
    1. Normalization is the process of minimizing redundancy and dependency by organizing fields and table of a database. The main aim of Normalization is to add, delete or modify field that can be made in a single table.
1. Types of Normalization
    1. First, Second, Third, Fourth
1. What is an index?
    1. a performance tuning method allowing faster retrieval of records from a table. It creates an entry for each value and it will be faster to retrieve data.

## Node JS

1. What is a first class function in Javascript?
    1. When functions can be treated like any other variable then those functions are first-class functions. There are many other programming languages, for example, scala, Haskell, etc which follow this including JS. Now because of this function can be passed as a param to another function(callback) or a function can return another function(higher-order function). map() and filter() are higher-order functions that are popularly used.

2. What is Node.js and how it works?
    1. Node.js is a virtual machine that uses JavaScript as its scripting language and runs Chrome’s V8 JavaScript engine. Basically, Node.js is based on an event-driven architecture where I/O runs asynchronously making it lightweight and efficient. It is being used in developing desktop applications as well with a popular framework called electron as it provides API to access OS-level features such as file system, network, etc.

3. How do you manage packages in your node.js project?
    1. It can be managed by a number of package installers and their configuration file accordingly. Out of them mostly use npm or yarn. Both provide almost all libraries of javascript with extended features of controlling environment-specific configurations. To maintain versions of libs being installed in a project we use package.json and package-lock.json so that there is no issue in porting that app to a different environment.

1. How many types of API functions are there in Node.js?
    1. There are two types of API functions:
        1. Asynchronous, non-blocking functions - mostly I/O operations which can be fork out of the main loop.
        1. Synchronous, blocking functions - mostly operations that influence the process running in the main loop.

## Docker

Docker Basic Questions
This category of Docker Interview Questions consists of questions that you’re expected to know. These are the most basic questions. An interviewer will start with these and eventually increase the difficulty level. Let’s have a look at them.

1. What is Hypervisor?

A hypervisor is a software that makes virtualization possible. It is also called Virtual Machine Monitor. It divides the host system and allocates the resources to each divided virtual environment. You can basically have multiple OS on a single host system. There are two types of Hypervisors:

Type 1: It’s also called Native Hypervisor or Bare metal Hypervisor. It runs directly on the underlying host system. It has direct access to your host’s system hardware and hence does not require a base server operating system.
Type 2: This kind of hypervisor makes use of the underlying host operating system. It’s also called Hosted Hypervisor.
2. What is virtualization?
Virtualization is the process of creating a software-based, virtual version of something(compute storage, servers, application, etc.). These virtual versions or environments are created from a single physical hardware system. Virtualization lets you split one system into many different sections which act like separate, distinct individual systems. A software called Hypervisor makes this kind of splitting possible. The virtual environment created by the hypervisor is called Virtual Machine.

3. What is containerization?
Let me explain this is with an example. Usually, in the software development process, code developed on one machine might not work perfectly fine on any other machine because of the dependencies. This problem was solved by the containerization concept. So basically, an application that is being developed and deployed is bundled and wrapped together with all its configuration files and dependencies. This bundle is called a container. Now when you wish to run the application on another system, the container is deployed which will give a bug-free environment as all the dependencies and libraries are wrapped together. Most famous containerization environments are Docker and Kubernetes.

4. Difference between virtualization and containerization

Once you’ve explained containerization and virtualization, the next expected question would be differences. The question could either be differences between virtualization and containerization or differences between virtual machines and containers. Either way, this is how you respond.

Containers provide an isolated environment for running the application. The entire user space is explicitly dedicated to the application. Any changes made inside the container is never reflected on the host or even other containers running on the same host. Containers are an abstraction of the application layer. Each container is a different application.

Whereas in Virtualization, hypervisors provide an entire virtual machine to the guest(including Kernal). Virtual machines are an abstraction of the hardware layer. Each VM is a physical machine.

5. What is Docker?
Since its a Docker interview, there will be an obvious question about what is Docker. Start with a small definition.

Docker is a containerization platform which packages your application and all its dependencies together in the form of containers so as to ensure that your application works seamlessly in any environment, be it development, test or production. Docker containers, wrap a piece of software in a complete filesystem that contains everything needed to run: code, runtime, system tools, system libraries, etc. It wraps basically anything that can be installed on a server. This guarantees that the software will always run the same, regardless of its environment.

6. What is a Docker Container?
Docker containers include the application and all of its dependencies. It shares the kernel with other containers, running as isolated processes in user space on the host operating system. Docker containers are not tied to any specific infrastructure: they run on any computer, on any infrastructure, and in any cloud. Docker containers are basically runtime instances of Docker images.

7. What are Docker Images?
When you mention Docker images, your very next question will be “what are Docker images”.

Docker image is the source of Docker container. In other words, Docker images are used to create containers. When a user runs a Docker image, an instance of a container is created. These docker images can be deployed to any Docker environment.

8. What is Docker Hub?
Docker images create docker containers. There has to be a registry where these docker images live. This registry is Docker Hub. Users can pick up images from Docker Hub and use them to create customized images and containers. Currently, the Docker Hub is the world’s largest public repository of image containers.

9. Explain Docker Architecture?
Docker Architecture consists of a Docker Engine which is a client-server application with three major components:

A server which is a type of long-running program called a daemon process (the docker command).
A REST API which specifies interfaces that programs can use to talk to the daemon and instruct it what to do.
A command line interface (CLI) client (the docker command).
The CLI uses the Docker REST API to control or interact with the Docker daemon through scripting or direct CLI commands. Many other Docker applications use the underlying API and CLI.
Refer to this blog, to read more about Docker Architecture.

10. What is a Dockerfile?
Let’s start by giving a small explanation of Dockerfile and proceed by giving examples and commands to support your arguments.

Docker can build images automatically by reading the instructions from a file called Dockerfile. A Dockerfile is a text document that contains all the commands a user could call on the command line to assemble an image. Using docker build, users can create an automated build that executes several command-line instructions in succession.

The interviewer does not just expect definitions, hence explain how to use a Dockerfile which comes with experience. Have a look at this tutorial to understand how Dockerfile works.

11. Tell us something about Docker Compose.
Docker Compose is a YAML file which contains details about the services, networks, and volumes for setting up the Docker application. So, you can use Docker Compose to create separate containers, host them and get them to communicate with each other. Each container will expose a port for communicating with other containers.

12. What is Docker Swarm?
You are expected to have worked with Docker Swarm as it’s an important concept of Docker.

Docker Swarm is native clustering for Docker. It turns a pool of Docker hosts into a single, virtual Docker host. Docker Swarm serves the standard Docker API, any tool that already communicates with a Docker daemon can use Swarm to transparently scale to multiple hosts.

13. What is a Docker Namespace?
A namespace is one of the Linux features and an important concept of containers. Namespace adds a layer of isolation in containers. Docker provides various namespaces in order to stay portable and not affect the underlying host system. Few namespace types supported by Docker – PID, Mount, IPC, User, Network

14. What is the lifecycle of a Docker Container?
This is one of the most popular questions asked in Docker interviews. Docker containers have the following lifecycle:
    1. Create a container
    1. Run the container
    1. Pause the container(optional)
    1. Un-pause the container(optional)
    1. Start the container
    1. Stop the container
    1. Restart the container
    1. Kill the container
    1. Destroy the container

15. What is Docker Machine?
    1. Docker machine is a tool that lets you install Docker Engine on virtual hosts. These hosts can now be managed using the docker-machine commands. Docker machine also lets you provision Docker Swarm Clusters.

