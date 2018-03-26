# mule-splitter-warning

Code to support blog : 
[Mule: Disable warning from splitter for For Each element](https://www.linkedin.com/pulse/mule-disable-warning-from-splitter-each-element-kedar-krishnan/)

To see the split warn message go to src/main/resources/log4j2.xml and comment below line and restart the application.
```java
<AsyncLogger name="org.mule.routing.ExpressionSplitter" level="ERROR"/>
```
After starting the mule application open web browser to:
1. For-each without WARN :+1: http://localhost:8081/start?values=1,2,3
2. For-each with WARN:-1: http://localhost:8081/start
