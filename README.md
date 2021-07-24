# maven-fundamentals
* Build section is where we make customized changes

### create a Maven project in Intellij
* New --> Project --> Maven --> select "Create from archetype" --> select "maven-archetype-quickstart"
* If not there, add maven archetype
  * groupId: org.apache.maven.archetypes
  * artifactId: maven-archetype-quickstart
  * version: 1.4
### Dependencies
https://maven.apache.org/guides/introduction/introduction-to-dependency-mechanism.html
* Scopes
  * compile
  * provided
  * runtime: opposite of provided. Dynamically loaded jar
  * test
  * system
  * import
* POM dependency

* If the project is copied. Need right click on pom.xml to "Add as a Maven Project" in Intellij

* Dependency Hierarchy in Intellij: in Maven view, expand dependencies
  
### Plugin Repository
* repository for plugins

### Plugins
* compiler plugin
  * invokes javac
  * defaults to older version of java: java 1.7
  * <configuration><release> to overwrite java version. Also for, memory, source/target
 * Jar plugin
 * Source plugin: package source code
   * Execution, goal, jar
 * Plugins vs PluginManagement. Use plugins. Use PluginManagement only in parent pom.
 * JavaDoc Plugin: Package phase
 
 
### Goals
* clean, compile, test, package, install, deploy
### Phases
* validate: Validate project and structure
* compile: compile the source code
* test: test the compiled code
* package: package the code in the specified package type
* integration-test: deploy and run integration tests
* verify: run checks to verify integrity
* install: install package in local repo
* deploy: copy package to remote repository
### convert a Java project to a Maven project
* create pom.xml file
* Reload project
* To load two maven projects in one Intellij window: Open one project, then go to Maven view and click on "+" to load the other project
