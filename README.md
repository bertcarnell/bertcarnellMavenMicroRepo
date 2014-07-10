bertcarnellMavenMircoRepo
=========================

[Maven Micro Repository](http://maven.apache.org/) for [bertcarnell](https://github.com/bertcarnell) java projects

### Include one of these repositories in your project


To include a repository in your project, add these sections to your <code>pom.xml</code>

``` xml
<project>
...
  <dependencies>
  ...
    <!-- Maven dependency, e.g. \releases\com\gmail\bertcarnell\AssertExtensions\1.0.1\AssertExtensions-1.0.1.jar -->
    <dependency>
      <!-- Deployed jar groupId -->
      <groupId>com.gmail.bertcarnell</groupId>
      <!-- Deployed jar filename -->
      <artifactId>AssertExtensions</artifactId>
      <!-- Desired version for the jar -->
      <version>1.0.1</version>
      <!-- Optional to set the scope of the dependency -->
      <scope>test</scope>
    </dependency>
  </dependencies>
  
  <repositories>
      <!-- user added repositories -->
      <repository>
          <!-- name for the repository (in Java) -->
          <id>bertcarnellMavenMicroRepo-releases</id>
          <!-- github url -->
          <url>https://raw.github.com/bertcarnell/bertcarnellMavenMicroRepo/master/releases</url>
          <!-- indicate this is a release repository -->
          <releases>
              <enabled>true</enabled>
          </releases>
          <snapshots>
              <enabled>false</enabled>
          </snapshots>
      </repository>
      <repository>
          <id>bertcarnellMavenMicroRepo-snapshots</id>
          <url>https://raw.github.com/bertcarnell/bertcarnellMavenMicroRepo/master/snapshots</url>
          <!-- indicate this is a snapshot repository -->
          <releases>
              <enabled>false</enabled>
          </releases>
          <snapshots>
              <enabled>true</enabled>
          </snapshots>
      </repository>
  </repositories>
</project>

```
