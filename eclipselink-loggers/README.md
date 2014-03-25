eclipselink-loggers
==================

* Author Ramon Lopez Viana (ramonlopezviana@gmail.com)

#Description
This module contains several logger implementations for eclipse link: jakarta commons logging, log4j & slf4j.
It's not my work. Just collected them from eclipselink wiki and included in this utility package.

#Installation
Just install through maven:
```
mvn install
```
#Usage
Declare dependency in the required project
```
      <dependency>
         <groupId>net.rlviana</groupId>
         <artifactId>eclipselink-loggers</artifactId>
      </dependency>
```

Include desired logger in eclipselink persistence configuration with eclipselink.logging.logger property:
- For slf4j:
``` 
eclipselink.logging.logger=org.eclipse.persistence.logging.Slf4jSessionLogger
```
- For log4j:
```
eclipselink.logging.logger=org.eclipse.persistence.logging.CommonsLoggingSessionLog
```

#Help
Refer to logging APIs for additional information.

#Credits
- Laurent Bourges (voparis)
- Miguel Angel Sosvilla Luis (msosvi) 

#References
- http://wiki.eclipse.org/EclipseLink/Examples/Foundation/Logging
- https://gist.github.com/msosvi/1325764/raw/50a882f881c2651f6de10cf661813faca22a480d/Slf4jSessionLogger.java
