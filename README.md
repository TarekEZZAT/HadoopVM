# HadoopVM
An Ubuntu VMWare/VirtualBox Hadoop project, with simple Map/Reduce example



Informations générales
Software
VMWare 16.1.0
Windows 10 (Machine hôte)
7zip
WinSCP
Ubuntu-18.04.5
Sur la machine virtuelle (Ubuntu-18.04.5)
java 1.8+
Hadoop-3.1.0
Eclipse jee-2020-06
Firefox

Utilisateurs/Mot de passe
dev (Utilisateur principal, sous le nom Ubuntu-18.04.5)/dev
hadoop (Utilisateur Hadoop)/hadoop

Quelques messages d’erreur possibles et leurs corrections
1/ Firefox 
Impossible de charger le profile firefox
sudo chmod -R 777 .mozilla
sudo chown -R $USER:$USER ~/.cache

URLs dans Hadoop
http://ubuntu:9870/dfshealth.html#tab-overview
http://ubuntu:9864/datanode.html
http://ubuntu:5249/node
http://ubuntu:5349/cluster

Hadoop Env (Linux)


export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
export PATH=$PATH:$JAVA_HOME/bin
export HADOOP_HOME=/usr/local/hadoop
export PATH=$PATH:$HADOOP_HOME/bin
export PATH=$PATH:$HADOOP_HOME/sbin
export HADOOP_CONF_DIR=/usr/local/hadoop/etc/hadoop
export HADOOP_CLASSPATH=/usr/lib/jvm/java-8-openjdk-amd64/lib/tools.jar
export PATH=$PATH:/home/hadoop/eclipse/jee-2020-06/eclipse

Hadoop Configuration
sudo apt install openjdk-8-jre-headless
ifconfig -a
ens33:
192.168.87.134
192.168.87.255

http://<VM_Public_IP>:5349. 
http://<VM_Public_IP>:5249. 

Ensure that ports 5349 and 5249 are open in Google VPC network -> Firewall.
