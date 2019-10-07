<h1>JBoss Jakarta EE Specs API</h1>
This project provides dependency management for a complete set of required APIs as defined by the Jakarta EE Platform Specifications.

This project goals:

<ul>
<li>Maintain a single repository containing the required APIs as defined by the Jakarta EE Platform Specification</li>
<indent>Having a consistent structure for all the Jakarta EE APIs make it easier to access, maintain, and consume.</indent>

<li>Individual release cycle per technology component</li>
<indent>Each API set can be released individually provides greater flexibility and control to the project owners without waiting for the aggregate to be released and integrated.  These API releases can be consumed by your project as a single dependency or as a fully defined set of required APIs for the profile.

<li>Define a naming scheme to associate the Specification version to the APIs contained in the JAR and distinguish between that and the release version of the artifact</li>
<indent>
The naming scheme adopted is as follows:
<ul>
<li>groupId:    org.jboss.spec + the package name
<li>artifactId: Technology-api_SpecVersion_spec
<li>version:    release version of the artifact
</ul>
</indent>
<li>Promote adoption of these spec-versioned APIs in all JBoss projects</li>
<indent>The APIs released from the org.jboss.specs project are certified for compliance to their respective specification.</indent>
</ul>

<h2>Jakarta EE Full Profile APIs</h2>
If you require the full set of required technology APIs defined by the Jakarta EE specification, add the following to your project pom.
<ul>
<li><code>&lt;groupId&gt;org.jboss.spec&lt;/groupId&gt;</code>
<li><code>&lt;artifactId&gt;jboss-jakartaee-8.0&lt;/artifactId&gt;</code>
<li><code>&lt;version&gt;<a href="https://repository.jboss.org/nexus/content/groups/public/org/jboss/spec/jboss-jakartaee-8.0/1.0.0.Final">1.0.0.Final</a>&lt;/version&gt;</code>
</ul>

<h2>Jakarta EE Web Profile APIs</h2>
If you are developing web applications and depend only on technologies that comprise the Jakarta EE Web Profile specification, you can opt to use the web profile pom.
<ul>
<li><code>&lt;groupId&gt;org.jboss.spec&lt;/groupId&gt;</code>
<li><code>&lt;artifactId&gt;jboss-jakartaee-web-8.0&lt;/artifactId&gt;</code>
<li><code>&lt;version&gt;<a href="https://repository.jboss.org/nexus/content/groups/public/org/jboss/spec/jboss-jakartaee-web-8.0/1.0.0.Final">1.0.0.Final</a>&lt;/version&gt;</code>
</ul>

<h2>Jakarta EE API UberJar</h2>
Else, if you prefer a jar containing the Jakarta EE API classes, that is also made available per a previous <a href="https://issues.jboss.org/browse/JBEE-73">feature request</a>.
<ul>
<li><code>&lt;groupId&gt;org.jboss.spec&lt;/groupId&gt;</code>
<li><code>&lt;artifactId&gt;jboss-jakartaee-8.0-all&lt;/artifactId&gt;</code>
<li><code>&lt;version&gt;<a href="https://repository.jboss.org/nexus/content/groups/public/org/jboss/spec/jboss-jakartaee-all-8.0/1.0.0.Final">1.0.0.Final</a>&lt;/version&gt;</code>
</ul>


These examples show the group:artifactId for use with Jakarta EE 8.    <a href="https://repository.jboss.org/nexus/content/groups/public/org/jboss/spec/">Releases</a> are available for Java EE 6, 7 and 8 also.
