Convert maven-properties into java-properties
=============================================

Example

    		<java.version>1.7</java.version>
    		<slf4j.version>1.7.6</slf4j.version>
    		<hsqldb.version>1.8.0.7</hsqldb.version>
    		
    		<project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
    		<project.reporting.outputEncoding>UTF-8</<project.reporting.outputEncoding>

ALgorithm

	1. Replace [</] with [@]
	2. Replace [@] with [  @]
	3. Replace RegEx [@.*version>\s] with []
	4. Replace [>] with [=]
	5. Drop blanks at the left 