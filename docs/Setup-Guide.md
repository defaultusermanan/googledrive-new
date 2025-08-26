# Setup Guide

Follow this guide to set up and run the `googledrive-new` Maven-based Java project.

---

## Prerequisites
Before you begin, ensure you have the following installed:

- **Java Development Kit (JDK)**: Version 8 or later.
- **Apache Maven**: Version 3 or later.
- **Git**: For repository cloning.

### Optional Tools
- Jenkins: For running CI/CD pipelines.
- A GitHub account configured with access to this repository.
---

## Step-by-Step Instructions

### 1. Clone the Repository
```bash
git clone <repository-url>
cd googledrive-new/java-hello-world-with-maven-master
```

### 2. Build the Project
Run Maven to compile classes.
```bash
mvn compile
```

### 3. Test the Project
Execute unit tests:
```bash
mvn test
```

### 4. Run the Application
Use the following Maven command to execute the `HelloWorld` entry point:
```bash
mvn exec:java -Dexec.mainClass="hello.HelloWorld"
```

### 5. CI/CD Pipelines
#### **GitHub Actions**
- Verify `CodeQL` workflows under `.github/workflows/codeql.yml`.

#### **Jenkins Integration**
- To use Jenkins, ensure `Jenkinsfile` is configured in your Jenkins instance.
- Adjust pipeline steps if necessary to suit your build environment.

---

## Troubleshooting
- **Build Errors**: Check dependencies in `pom.xml` and ensure the proper JDK/Maven versions are installed.
- **Test Failures**: Inspect test logs for detailed error messages.
- For additional support, refer to the project's `README.md` or contact the repository maintainer.