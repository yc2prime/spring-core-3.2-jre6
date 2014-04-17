spring-core-3.2-jre6
====================

Spring-core-3.2.8 source and binary for JRE 6

For some cloud service such as [Sina App Engine (SAE)](http://sae.sina.com.cn "SAE"), the JRE is still at version 6, which is not compatible for many utilities compiled by JDK 1.7. Here is the spring-core-cglib for JRE 6. 

>spring-data-mongodb-1.4 depends on this package. I used spring-core-2.8.3-RELEASE.jar (it has included this package but compiled with JDK 7) on SAE and failed. So I want to share these sources to help others who have similar problems.

spring-core-3.2-jre6 (中文版)
=====================
JDK 8已经发布了，可是国内的很多云计算平台还停留在JRE 6的阶段，其中包括做的还不错的[Sina App Engine (SAE)](http://sae.sina.com.cn "SAE")。可是JRE 6的环境里面很多JDK 7编译的class是不能运行的，比如spring 官方提供的3.2之后的版本。这里我们提供了spring-core-cglib 3.2的源代码以及使用JDK 6编译的jar，经SAE实测可以使用。

>最近一个项目的决定移植到SAE上，其中的一个包spring-data-mongodb-1.4依赖spring-core-3.2,可是Spring官方的jar包是JDK 7编译的，放到SAE上连JVM都启动不起来。于是我们找到了其中的关键依赖——cglib的源代码，使用JDK 6进行编译，终于使得程序正常运行在SAE上了。我们决定把代码放到GitHub上，希望能为遇到类似问题的同行提供帮助。
