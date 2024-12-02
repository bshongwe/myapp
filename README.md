# MyApp 🚀

![Visits Badge](https://badges.pufler.dev/visits/bshongwe/myapp)
![GitHub Repo Stars](https://img.shields.io/github/stars/bshongwe/myapp)
![GitHub Forks](https://img.shields.io/github/forks/bshongwe/myapp)
![GitHub Issues](https://img.shields.io/github/issues/bshongwe/myapp)
![GitHub License](https://img.shields.io/github/license/bshongwe/myapp)


Welcome to **MyApp**, a sample Java application designed to demonstrate a robust CI/CD pipeline with tools for code quality, security, and continuous deployment.

## 🌟 Features

- 📦 **Modular Java Application** - Simple setup for demonstration purposes
- 🐋 **Dockerized** - Runs smoothly in a containerized environment
- ☸️ **Kubernetes-Ready** - Deployable to Kubernetes clusters using Helm
- 🔒 **Automated Security Scanning** - Integrates OWASP ZAP for enhanced security
- 🧩 **Code Quality Analysis** - Configured with SonarQube for maintaining quality
<br></br>

## ⚙️ Requirements

To build and run MyApp locally, ensure you have the following installed:

- Java 11 or higher
- Docker
- Kubernetes and Helm (for container orchestration)
- Maven (for dependency management)
<br></br>

## 🚀 Getting Started

Follow these steps to set up MyApp on your local machine:

1. **Clone this repository**:
   ```bash
   git clone https://github.com/bshongwe/myapp.git
   cd myapp
   ```

2. **Build the Project**:
   ```bash
   mvn clean install
   ```

3. **Run the Application**:
   ```bash
   java -jar target/my-app-1.0.0.jar
   ```

   Alternatively, to run within Docker:
   ```bash
   docker build -t myapp .
   docker run -p 8080:8080 myapp
   ```

<br></br>
## 📊 Monitoring & Quality Checks

MyApp is configured with SonarQube and OWASP ZAP for code quality and security scanning.

- **SonarQube**: Runs static code analysis to detect code smells, bugs, and security vulnerabilities.
- **OWASP ZAP**: Scans for security issues in the application.
<br></br>

### 📝 Code Quality Report

To generate a SonarQube report:
```bash
mvn sonar:sonar -Dsonar.projectKey=my_project -Dsonar.host.url=http://localhost:9000 -Dsonar.login=${SONAR_TOKEN}
```
<br></br>

## 🏗️ Deployment

MyApp is ready for deployment to Kubernetes using Helm. Customize the deployment as needed in the `helm/` directory.

1. **Package the Helm Chart**:
   ```bash
   helm package helm/my-app
   ```

2. **Deploy to Kubernetes**:
   ```bash
   helm install my-app ./my-app-1.0.0.tgz
   ```


---

```
Happy Coding! 👨‍💻👩‍💻
```

---

### Key sections to learn from this:

1. **Features** - Highlights the core attributes of the application.
2. **Requirements** - Lists necessary tools for setup.
3. **Getting Started** - Provides basic setup instructions to get the app running locally or in Docker.
4. **Monitoring & Quality Checks** - Briefs users on quality and security tools in use.
5. **Deployment** - Guides on deploying the app using Helm and Kubernetes.
6. **License** - Specifies the project license.
