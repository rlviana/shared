build-qa
==================
* Author Ramon Lopez Viana (ramonlopezviana@gmail.com)

#Description
<!-- Comments -->
This maven project contains configuration related to Code Quality Assurance tasks. Includes configuration for the following tools:
- eclipse
- pmd
- checkstyle
- findbugs 

#Usage
If used in maven, this must be included as a dependency in the project and extract them to the required place.
```
		<dependency>
			<groupId>net.rlviana</groupId>
			<artifactId>build-qa</artifactId>
			<version>${build-tools.version}</version>
			<classifier>resources</classifier>
			<type>zip</type>
			<!-- Make sure this isn't included on any classpath -->
			<scope>provided</scope>
		</dependency>
``` 
Since it contains several configuration files. The plugins using them must reference them to use it.
 
#Help
Refer to maven plugin documentation & eclipse docs for additional information.
An example of its use can be found in my blog (http://rlviana.wordpress.com)

#Credits
Created by rlviana

#References
- http://www.maven.org
- http://rlviana.wordpress.com/tag/findbugs/
- http://rlviana.wordpress.com/tag/checkstyle/
- http://rlviana.wordpress.com/tag/pmd/
