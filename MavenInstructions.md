These are the instructions for publishing HELM GitHub repositories to Maven. All projects have to be signed with PGP. 

 

Find the Key: 
The project keys are kept by the Pistoia Alliance technical support group. Contact info@openHELM.org for details. 

Deploy with apache maven:
The pom.xml  must be extended to generate javadoc and sources attachments and integrate the maven-gpg-plugin, so that the artifacts can be signed using maven. 

For the documentation, see http://central.sonatype.org/pages/apache-maven.html and http://central.sonatype.org/pages/requirements.html. 

 

To deploy a snapshot, just add -SNAPSHOT to the version, see 

      <groupId>org.pistoiaalliance.helm</groupId>

      <artifactId>helm2-helmnotationparser</artifactId>

      <version>1.0.0-SNAPSHOT</version>

      <packaging>jar</packaging>


Run maven with clean deploy and the snapshot version will be uploaded to the snapshot repository. 

 

Steps to run maven:
 

1)   Add the keys to your gpg with the import function: „gpg –import pistoia_pub.gpg“ and „gpg –import pistoia_sec.gpg“

2)   Add the following to your maven settings

 

<settings>

<profiles>

    <profile>

      <id>helm</id>

      <activation>

        <activeByDefault>true</activeByDefault>

      </activation>

      <properties>

        <gpg.executable>gpg</gpg.executable>

        <gpg.passphrase>macromol2013</gpg.passphrase>

      </properties>

    </profile>

  </profiles>

  <servers>

    <server>

      <id>helm</id>

      <username>PistoiaHELM</username>

      <password>macromol2013</password>

    </server>

  </servers>

</settings>

 

3)   Run maven with clean deploy. 

 
