# Programmation fonctionnelle avancée (Scala, Apache Spark)

## Objectifs
Dans ce cours nous allons :

* Voir les bases de la programmation fonctionnelle en Scala,
* Apprendre à manipuler les concepts avancées de collections, classes, higher-order functions, pattern matching, mapReduce etc.
* Developper des programmes paralleles avec Apache Spark pour le pré-traitement des données dans un cluster Hadoop
* Etudier comment assurer le chargement, l'extraction et la transformation des données avec Spark Dataframe, SQL et Datasets.
* Traiter de données en Streaming
* Developper des modèles Machine Learning en utilisant la Spark MLlib

## Installation de Scala

Vous pouvez installer Scala à partir de :

* Scala REPL (https://www.scala-lang.org/download/)
* sbt (https://www.scala-sbt.org/download.html)
* IntelliJ (https://www.jetbrains.com/idea/)
* jupyter notebook avec almond (https://almond.sh/docs/quick-start-install)

## Installation de Apache Spark

* Installer Java JDK (11 ou 8)(https://adoptopenjdk.net/)
* Télécharger Apache spark 2.4.7 (https://spark.apache.org/downloads.html)
* Deplacer le spark-2.4.7*.zip dans le votre home
    * `mv spark-2.4.7*.zip $HOME`
    * `cd $HOME`
    * `unzip spark-2.4.7*.zip`
    * `mv spark-2.4.7* spark-2.4.7`
* Créer une variable d'environnement SPARK_HOME dans .bashrc ou bash_profile
    * `export SPARK_HOME=$HOME/spark-2.4.7`
    * `export PATH=SPARK_HOME/bin:$PATH`
    * `source .bashrc`

* créer un environnement virtual python dans conda
    * `conda env create -f environment.yml`
* Installer spylon-kernel pour connecter jupyter avec Spark-shell
    * `cd $HOME`
    * `python -m spylon_kernel install --user`
* Démarrer jupyter notebook ou jupyter lab pour tester

* Vous pouvez aussi créer un compte Databricks (https://databricks.com) pour travailler dans un cluster Spark en mode Try.
