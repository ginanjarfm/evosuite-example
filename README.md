# Evosuite Example

## Description

This project is an example of Evosuite IntelliJ IDEA projects . The detail can be found at [Evosuite Documentation IntelliJ IDEA plugin](http://www.evosuite.org/documentation/intellij-idea-plugin/)

+ IntelliJ IDEA Community Edition IC-201.7223.91
+ OpenJDK Runtime Environment (AdoptOpenJDK)(build 1.8.0_252-b09)
+ Apache Maven 3.6.3
+ Evosuite Standalone 1.0.6

### Maven

[Maven Project](https://github.com/ginanjarfm/evosuite-example/tree/master/EvosuiteMaven)

```bash
%M2_HOME%/bin/mvn  compile  evosuite:generate  \
  -Dcores=1  \
  -DmemoryInMB=2000  \
  -DtimeInMinutesPerClass=3  \
  -DspawnManagerPort=63858  \
  -Dcuts=org.example.Foo_ESTest_scaffolding,org.example.Foo_ESTest,org.example.Foo  \
  evosuite:export  -DtargetFolder=src/test/java
```

<img src="https://raw.githubusercontent.com/ginanjarfm/evosuite-example/master/media/maven-dialog.png"/>

### Gradle

[Gradle Project](https://github.com/ginanjarfm/evosuite-example/tree/master/EvosuiteGradle)

```bash
%JAVA_HOME%/bin/java  -jar  %EVOSUITE_DIR%/evosuite-1.0.6.jar  \
  -continuous  execute  \
  -Dspawn_process_manager_port=65210  \
  -Dctg_memory=2000  \
  -Dctg_cores=1  \
  -Dctg_time_per_class=3  \
  -Dctg_export_folder=../../src/test/java  \
  -Dctg_selected_cuts=org.example.Foo  \
  -DCP_file_path=/var/folders/j1/1x10bdrs3zj78fy_ht73p3800000gn/T/EvoSuite_ctg_classpath_file176106161814374871.txt
```

<img src="https://raw.githubusercontent.com/ginanjarfm/evosuite-example/master/media/gradle-dialog.png"/>

## Author

Author: [Ginanjar Fahrul M](https://www.upwork.com/freelancers/~015c944ce8d84e104c)
