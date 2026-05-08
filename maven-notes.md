# Maven  

```text 
# What is Maven ?


- Build Management: Maven handles compiling, testing, packaging, and deploying code. It automates the build process
- Dependency Management: Maven automatically manages external libraries or dependencies that a project needs
- Project Structure: Maven enforces a standard directory structure for projects, making it easier for developers to understand how a project is organized, 
  regardless of who wrote the code  
- Repositories: Maven uses repositories
  1. Central / Remote Repostiories
  2. Local Repository
- Plugins: Maven supports plugins to perform various tasks like compiling code, running tests, generating reports, and more
- pom.xml (Project Object Model): The pom.xml file is the heart of a Maven project. It contains configuration information like dependencies, build settings, 
   and plugin definitions.
   



#  What is pom. xml ?
POM = Project Object Model

It is the core configuration file of Maven project.It conatins-:
→ Project information
→ Dependencies
→ Plugins
→ Build configuration
→ Repositories


#  Important Note about Maven -

# What is Archetype?
An archetype in Maven represents a template for generating a project. It’s a way to create a project with a predefined structure. Some common archetypes include:

- quick-start: This is a basic template for a simple console application. It usually includes a simple structure with one class to get you started.
-web-app: This archetype is used to create a web application project. It sets up the necessary files and structure for a web-based project, often including directories for WEB-INF, and configurations for servlets, JSPs, etc.

# What is groupId? 
- The groupId is a unique identifier for the group or organization that is creating the project. It typically represents the domain name of the company or the organization in reverse. This helps in distinguishing projects between different organizations.

Examples:
com.cisco
in.amazon
com.hcl

# what is artifact ?
In Maven, an artifact refers to a file, typically a JAR, WAR, or other types of compiled code, that is produced by a Maven project. It is the primary output of a build process

1. Artifact ID: A unique identifier for the artifact
2. Group ID: A unique identifier for the group or organization that is responsible for the artifact.

Version:
The version refers to the version of your project or artifact. This can indicate the maturity and stability of the project:

SNAPSHOT: This indicates that the project is still under development and is not yet finalized. It’s a work-in-progress version.
RELEASE: This version has been finalized and is ready for production or delivery to clients. It’s stable and no longer changing.

Note: Artifacts are stored in repositories (like Maven Central or private repositories(NEXUS / JFROG)) and can be dependencies for other project



# What are the types of Repositories?

There are three types of repositories:

1. Central Repository (Public): This is the default public repository provided by Maven, containing a huge collection of popular libraries and frameworks.
   When you declare a dependency in your pom.xml, Maven looks here first.

2. Remote Repository (Private): Companies or teams might set up their own private repositories (e.g., using tools like Nexus or JFrog) to store internal
   libraries, proprietary software, or to maintain versions of their own code.

3. Local Repository (.m2 directory): This is your personal local repository on your machine. When Maven downloads dependencies, they are cached here to
   avoid downloading them repeatedly. The default location for this local repository is typically ~/.m2/repository.

