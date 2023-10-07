<h2>Installation de Hadoop 2.7 sur Linux</h2>
<hr/>

<h3>1. Télécharger JAVA </h3>
<br/>
<h4>- Taper commande : sudo apt-get update</h4>
<img src="./img/img01.png">
<br/><br/>
<h4>- Taper la commande suivante en pour installer JAVA 11 : sudo apet-get install default-jdk</h4>
<img src="./img/img02.png">
<br/><br/>
<img src="./img/img03.png">
<br/><br/>
<h4>Taper ensuite la commande java -version pour vérifier si java a été bien installée : java -version</h4>
<img src="./img/img04.png"/>
<h3>2. Installer Open SSH Client et Open SSH Server/h3>
<h4>sudo apt-get install openssh-server openssh-client</h4>
<h3>3. Générer des paires de clés privées et publiques : ssh-keygen -t rsa -P ""</h3>
<img src="./img/img05.png"/>
<br/><br/>
<h3>4. Configurer SSH sans mot de passe : cat /home/lehcene/rsa_key.pub >> /home/lehcene/authorized_keys</h3>
<img src="./img/img06.png"/>
</br></br>
<h3>5. Vérifier sur localhost par SSH</h3>
<img src="./img/img07.png"/>
<h3>6. Télécharger et installer hadoop 2.7.1</h3>
<h4>- commande télécharge hadoop : wget https://archive.apache.org/dist/hadoop/common/hadoop-2.7.1/hadoop-2.7.1.tar.gz</h4>
<img src="./img/img08.png"/>
<img src="./img/img09.png"/>

<h4>- Puis extraire le dossier en utilisant la commande suivante : tar xzf hadoop-2.7.1.tar.gz</h4>
<h4>- Fiare une Modification sur le Fichiers : bashrc, hadoop-env.sh, core-site.xml, yarn-site.xml, mapred-site.xml.template, copier le fichier mapred-site.xml.template au mapred-site.xml , mapred-site.xml,hdfs-site.xml</h4>
<img src="./img/img010.png"/>
<h3>7. Démarrer le cluster</h3>
<h4>- Formater le Name Node avec la commande suivante : hsfs namenode -format</h4>
<img src="./img/img010.png"/>
<br/><br/>
<img src="./img/img011.png"/>
<h3>- Démarrer les services HDFS avec la commande suivante : start-dfs.sh</h3>

<img src="./img/img012.png"/>
<br/><br/>
<img src="./img/img013.png"/>
<h3>- Démarrer les services YARN avec la commande suivante : start-yarn.sh</h3>
<img src="./img/img014.png"/>
<h3>- Vérifier si les services ont été démarrés avec la commande jps :</h3>
<img src="./img/img015.png"/>
<h3>7- Conulter Hadoop 2.7.1 via Web avec address : localhost:50070</h3>
<img src="./img/img016.png"/>