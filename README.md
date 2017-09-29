# Performance tests for [HDTQ](https://github.com/JulianRei/hdtq-java)

## Overview

Executes quad pattern queries as generated by the [HDT query generator](https://github.com/JulianRei/hdtq-java-queryGeneration) against HDTQ, Jena and Virtuoso.

## Prerequisites

Add [HDTQ](https://github.com/JulianRei/hdtq-java) to your local Maven repository.

Add to project dependencies (Both can be found [here](http://vos.openlinksw.com/owiki/wiki/VOS/VOSDownload#Jena%20Provider).):
1. Virtuoso Jena 3.0.x Provider JAR file.
2. Virtuoso JDBC 4 Driver JAR file.

## Compiling

Use mvn install to let Apache Maven install the required jars in your system.

## Usage

1. Import RDF data into HDTQ or Jena TDB or Virtuoso.
2. Start the performance test (e.g. via Eclipse or via terminal: java -jar performanceTest.jar) to see input parameters.

Example of use:
```
java -jar some/path/performanceTest.jar -f some/where/BEARdayAT.hdt -o ~/results/ -q ~/some/place/BEARday/queries/ -r 3 -p SPOG SPOV
```

## License

LPGL

## Authors

Julian Reindorf <julian.reindorf@gmailcom>