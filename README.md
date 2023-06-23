 --- Unix ---
#complie
javac -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar com/ibm/mq/samples/jms/JmsGet.java

javac -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar com/ibm/mq/samples/jms/JmsPut.java

javac -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar com/ibm/mq/samples/jms/JmsPutDebt.java

javac -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar ./com/ibm/mq/samples/jms/JmsGetDebt.java

----
## Run 
java -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar:. com.ibm.mq.samples.jms.JmsGet

java -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar:. com.ibm.mq.samples.jms.JmsPut

java -cp ./com.ibm.mq.allclient-9.3.0.0.jar:./javax.jms-api-2.0.1.jar:./json-20220320.jar:. com.ibm.mq.samples.jms.JmsPutDebt


 --- Windows -- 
## Compile
javac -cp "./com.ibm.mq.allclient-9.3.0.0.jar;./javax.jms-api-2.0.1.jar;./json-20220320.jar" ./com/ibm/mq/samples/jms/JmsPutGet.java

###Run 
java -cp "./com.ibm.mq.allclient-9.3.0.0.jar;./javax.jms-api-2.0.1.jar;./json-20220320.jar" com.ibm.mq.samples.jms.JmsPutGet


----- 
#For Node js
install -> https://github.com/Microsoft/nodejs-guidelines/blob/master/windows-environment.md#environment-setup-and-configuration

run 
node test_https.js
