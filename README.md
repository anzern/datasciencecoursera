# datasciencecoursera
cd to kafka folder

First start Zoomkeeper 

.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties


--------- then open another CMD and start kafka 

.\bin\windows\kafka-server-start.bat .\config\server.properties


--------- then open another CMD and create kafka topic

.\bin\windows\kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic analyticsvidya


---------- to see the created topic

.\bin\windows\kafka-topics --list --zookeeper localhost:2181
