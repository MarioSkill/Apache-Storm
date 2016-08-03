Dockerizing Apache-Storm 
======
**Docker**  Apache Storm.
<br><br>
Instala todos los componentes necesarios para ejecutar Apache Storm
* Storm 1.0.1
* ZOO 3.4.8
* ZQQ 4.1.5
* Java 8

#### Screenshot
![Screenshot software](http://storm.apache.org/images/logo.png "screenshot software")

## Download
* [Version 1](https://github.com/MarioSkill/Apache-Storm/archive/master.zip)

## Usage
```docker run --name STORM_11_07_2016_46_870c2049c1a9c326a71f75cec66fd6e8 -m 4880m -v /var/www/default/TFG2/src/BenchmarkBundle/Resources/public/tfg/resources/:/bigData/ -dit ubuntu-storm:latest /bigData/medir_STORM.sh```

## MEDIR_STORM.SH 
```
/usr/local/src/apache-storm-$STORM_VERSION/bin/storm nimbus&
/usr/local/src/apache-storm-$STORM_VERSION/bin/storm supervisor&
/usr/local/src/zookeeper-$ZOO_VERSION/bin/zkServer.sh start
```

## Contacto
* e-mail: mario.vasilecabezas@gmail.com
* Twitter: [@MarioSkill](https://twitter.com/MarioSkill "twitterhandle on twitter")
