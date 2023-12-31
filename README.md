# Docker Container run IBM MQ Server
## Install MQ Server on Docker
```
docker pull icr.io/ibm-messaging/mq:latest
docker volume create qm1data
```


```
 docker run --env LICENSE=accept --env MQ_QMGR_NAME=QM1 --volume qm1data:/mnt/mqm --publish 1414:1414 --publish 9443:9443 --detach --env MQ_APP_PASSWORD=passw0rd --name QM1 icr.io/ibm-messaging/mq:latest
```

```
docker exec -ti QM1 bash
dspmqver
dspmq
```
 
 
 --- Unix ---
## complie
```
javac -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar com/ibm/mq/samples/jms/JmsGet.java

javac -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar com/ibm/mq/samples/jms/JmsPut.java

javac -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar com/ibm/mq/samples/jms/JmsPutDebt.java

javac -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar ./com/ibm/mq/samples/jms/JmsGetDebt.java
```

----
## Run 
```
java -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar:. com.ibm.mq.samples.jms.JmsGet

java -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar:. com.ibm.mq.samples.jms.JmsPut

java -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar:. com.ibm.mq.samples.jms.JmsPutDebt
```

 ---Java on  Windows -- 
## Compile
```
javac -cp "./com.ibm.mq.allclient-9.3.0.0.jar;./javax.jms-api-2.0.1.jar;./json-20220320.jar" ./com/ibm/mq/samples/jms/JmsPutGet.java
```

### Run 
```
java -cp ".;./com.ibm.mq.allclient-9.3.0.0.jar;./javax.jms-api-2.0.1.jar;./json-20220320.jar" com.ibm.mq.samples.jms.JmsPutGet

java -cp ".;./com.ibm.mq.allclient-9.3.0.0.jar;./javax.jms-api-2.0.1.jar;./json-20220320.jar" com.ibm.mq.samples.jms.JmsPutDebt
```


----- 
# For Node js
install -> https://github.com/Microsoft/nodejs-guidelines/blob/master/windows-environment.md#environment-setup-and-configuration

## run using REST API (port 9443)
```
node rest_https_put.js 
node rest_https_gut.js 
```

## Run using node library (port 1443)
```
node amqsput.js
node amqsget.js
```


## REST API 
# with postman
import ./rest_api/IBM_MQTT.poetman_collection.json -->  postman 