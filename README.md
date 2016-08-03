# Apache-Storm
How to Start Docker 

docker run --name nameID -m 4880m -v /var/www/default/TFG2/src/BenchmarkBundle/Resources/public/tfg/resources/:/bigData/ -dit ubuntu-storm:latest /bigData/medir_STORM.sh

---- < MEDIR_STORM.SH > ---- 
#!/bin/bash
/usr/local/src/apache-storm-$STORM_VERSION/bin/storm nimbus&
/usr/local/src/apache-storm-$STORM_VERSION/bin/storm supervisor&
/usr/local/src/zookeeper-$ZOO_VERSION/bin/zkServer.sh start

---- </ MEDIR_STORM.SH > ---- 