# Jenkins Basics

## Index

1. What Jenkins is
2. Why Jenkins matters in DevOps
3. Jenkins architecture
4. Installation and setup
5. Jobs and builds
6. Plugins and extensibility
7. Credentials and security
8. Build agents and executors
9. CI workflow in Jenkins
10. Common benefits and limitations
11. Best practices
12. Typical interview points

## 1. What Jenkins is

Jenkins is an open-source automation server used to build, test, and deploy software. It is one of the most widely used tools in continuous integration and continuous delivery because it helps teams automate repetitive tasks and reduce manual errors. In simple terms, Jenkins acts as a coordinator that runs workflows whenever developers push code or trigger a build manually.

### Subtopics

- Automation server
- Open-source and extensible
- Popular in CI/CD pipelines
- Integrates with Git, Maven, Gradle, Docker, and cloud tools

## 2. Why Jenkins matters in DevOps

Jenkins matters because it connects development and operations through automation. Instead of waiting for manual testing and deployment, teams can get fast feedback, detect errors early, and release software more frequently. This is essential in DevOps because speed, reliability, and consistency are all critical.

### Subtopics

- Faster feedback
- Reduced human error
- Repeatable builds
- Standardized deployment steps

## 3. Jenkins architecture

The Jenkins architecture is built around a controller and worker nodes. The controller is the main server that manages jobs, scheduling, and overall configuration. Worker nodes, often called agents, perform the actual build tasks. This separation allows teams to distribute workload and run jobs across different machines or environments.

### Subtopics

- Master/controller
- Agent/node
- Executors
- Distributed builds

## 4. Installation and setup

A basic Jenkins installation usually involves installing Java first, then downloading Jenkins and starting the service. After startup, you open the web UI, unlock Jenkins using the initial admin password, and install recommended plugins. Once configured, you create jobs and connect repositories.

### Subtopics

- Java dependency
- Initial setup wizard
- Plugin installation
- Admin user creation
- URL and security configuration

## 5. Jobs and builds

Jenkins jobs are the core units of work. A job can be a build, a test run, a deployment, or a scheduled task. Each job uses a defined set of steps, such as checking out code, compiling source, running tests, and packaging artifacts. Jenkins supports freestyle projects and pipeline projects, depending on the level of complexity.

### Subtopics

- Freestyle jobs
- Pipeline jobs
- Build triggers
- Console output
- Build history

## 6. Plugins and extensibility

One of Jenkins’s most powerful features is its plugin ecosystem. Plugins expand Jenkins beyond its core capabilities, allowing integration with GitHub, Slack, Docker, Kubernetes, AWS, SonarQube, and many testing tools. This makes Jenkins flexible enough for both small teams and enterprise-grade automation pipelines.

### Subtopics

- Plugin manager
- Official and community plugins
- GitHub plugin
- Docker plugin
- Slack or email notifications

## 7. Credentials and security

Security is important in Jenkins because it often deals with code repositories, deploy credentials, and server access. Jenkins lets administrators store secrets securely, manage users and permissions, and restrict who can create or run jobs. Proper configuration prevents accidental exposure of sensitive information.

### Subtopics

- Credentials store
- Secret text and SSH keys
- User roles
- Matrix-based security
- Least privilege principle

## 8. Build agents and executors

Build agents are separate machines that perform compute-intensive work for Jenkins. Executors are the number of concurrent jobs an agent can run. Using agents improves performance, isolates workloads, and allows you to run builds in different environments, such as Linux, Windows, or Docker containers.

### Subtopics

- Agent labels
- SSH agents
- Docker-based agents
- Parallel execution
- Resource allocation

## 9. CI workflow in Jenkins

A typical CI workflow in Jenkins starts when code is pushed to a repository. Jenkins detects the change, checks out the repository, runs tests, and reports results. If the build passes, the team can move forward to deployment or further validation. This loop is important because it provides fast feedback to developers before issues become costly.

### Subtopics

- Source control trigger
- Build stage
- Test stage
- Report generation
- Failure notifications

## 10. Common benefits and limitations

Jenkins offers strong flexibility and a large ecosystem, but it also has some challenges. It can be complex to maintain if too many plugins are installed, and its UI may feel old compared to newer tools. Still, for many organizations, Jenkins remains a dependable choice for automation because of its maturity and broad adoption.

### Subtopics

- Benefits: flexibility, mature ecosystem, free and open source
- Limitations: plugin sprawl, maintenance overhead, configuration complexity
- Good for custom workflows
- Requires careful administration

## 11. Best practices

To use Jenkins effectively, teams should keep configurations simple, use pipeline-as-code, and avoid unnecessary plugin installation. Naming conventions, version control for Jenkinsfiles, and clear role-based permissions make larger environments easier to manage. A well-maintained Jenkins estate is easier to scale and troubleshoot.

### Subtopics

- Use pipeline as code
- Keep jobs modular
- Use environment variables
- Back up configuration
- Monitor plugin health

## 12. Typical interview points

Jenkins is a common topic in DevOps interviews because it is widely used and demonstrates practical automation knowledge. Interviewers usually ask about jobs, pipelines, plugins, agent configuration, build triggers, and troubleshooting failed builds. Understanding these concepts shows that you can work with real CI/CD systems.

### Subtopics

- Declarative pipeline
- Build trigger types
- Artifact handling
- Blue Ocean
- Jenkinsfile basics
