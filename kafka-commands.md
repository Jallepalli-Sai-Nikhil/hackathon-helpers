cd C:\kafka

java -version

bin\windows\kafka-storage.bat random-uuid


format
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-storage.bat format -t <CLUSTER_ID> -c config\server.properties


start
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-server-start.bat config\server.properties

create a topic
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-topics.bat --create --topic user-created --bootstrap-server localhost:9092

list all topics
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-topics.bat --list --bootstrap-server localhost:9092


describe a topic
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-topics.bat --describe --topic user-created --bootstrap-server localhost:9092

delete topic
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-topics.bat ^
--delete ^
--topic user-created ^
--bootstrap-server localhost:9092



produce message
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-console-producer.bat ^
--topic user-created ^
--bootstrap-server localhost:9092



consumer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-console-consumer.bat ^
--topic user-created ^
--from-beginning ^
--bootstrap-server localhost:9092

Consume latest message
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-console-consumer.bat ^
--topic user-created ^
--bootstrap-server localhost:9092


list consumer groups
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bin\windows\kafka-consumer-groups.bat ^
--bootstrap-server localhost:9092 ^
--list
















