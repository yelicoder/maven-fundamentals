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
  
### Plugin Repository
* repository for plugins
