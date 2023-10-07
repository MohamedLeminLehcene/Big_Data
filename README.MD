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