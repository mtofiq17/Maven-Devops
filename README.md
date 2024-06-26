# Maven-DevOps

## Setup in Ubuntu Ec2
- **Update Packages**: sudo apt update -y
- **Install Java**: sudo apt install openjdk-11-jre -y
- **Install Java**: sudo apt-get install maven -y

## Maven Build Lifecycle

Maven has three built-in build lifecycles: clean, default, and site.

- **Clean Lifecycle**: Deletes any build output generated by previous builds.
  - `clean`: Deletes any build output generated by previous builds.

- **Default Lifecycle**:
  - `validate`: Validates the project structure and verifies if all necessary information is available.
  - `compile`: Compiles the project's source code.
  - `test`: Runs unit tests against compiled source code.
  - `package`: Packages the compiled code into a distributable format (e.g., JAR, WAR).
  - `install`: Installs the package into the local repository for use as a dependency in other projects (`.m2`).
  - `deploy`: Deploys the package to a remote repository for sharing with other developers or environments (Push to Nexus).

- **Site Lifecycle**:
  - `site`: Generates project documentation and reports.
  - `site-deploy`: Deploys the generated documentation to a remote web server.

### Maven Command Examples:

Here are some common Maven commands:

- `mvn compile`: Compiles the project's source code.
- `mvn test`: Runs unit tests against compiled code.
- `mvn package`: Packages the compiled code into a distributable format.
- `mvn install`: Installs the package into the local repository.
- `mvn deploy`: Deploys the package to a remote repository.
- `mvn site`: Generates project documentation and reports.
- `mvn site-deploy`: Deploys the generated documentation to a remote web server.  
- `mvn clean`: Executes the clean phase, deleting any previous build outputs.

## Run Application
- `Run application command`: java -jar target/spring-boot-web.jar
