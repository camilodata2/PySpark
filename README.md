# ❤️ PYSPARK
is an Apache Spark compatible programming language that can be used to build various data platforms and manage data analytics -
big data is a Python API developed as part of the collaboration between Apache Spark

## 🤤 How to install Spark
There are many way to install spark but i'm gonna show you how to install in two way, the first way is throug out a simple way just opening your notebook
on google or in your machine, and fallow the below steps
1. [!apt-get install openjdk-8-jdk-headless -qq > /dev/null](#id1)
2. [!wget -q http://apache.osuosl.org/spark/spark-3.0.0/spark-3.0.0-bin-hadoop3.2.tgz](#id2)
3. [!tar xf spark-3.0.0-bin-hadoop3.2.tgz](#id3)
4. [!pip install -q findspark](#id4)

### 🙃 Set Environment Variables

Once the above commands are executed, It is time to add relevant paths to the environment. You can manage multiple versions of spark by pointing-
to the correct version through environment variables. Run below set of commands to point to Apache Spark 3.0.0 version downloaded earlier.
1. [import os](#id1)
2. [os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-8-openjdk-amd64"](#id2)
3. [os.environ["SPARK_HOME"] = "/content/spark-3.0.0-bin-hadoop3.2"](#id3)

#### 🤓 Quick Installation Test

Now it is time to test our spark installation and the version of it
We should be able to use Spark 3.0.0 version and pyspark with a 3.0.0 version as well.

1. [import findspark](#id1)
2. [findspark.init()from pyspark.sql import SparkSession](#id2)
3. [spark = SparkSession.builder.master("local[*]").getOrCreate()](#id3)

##### 🐳 Spark with docker
The other way to install Spark is with docker, in my opinion it is the best way to install Spark on your machine, maybe you are thinking that you have to know about
docker but it's not true you just need to go to the following website https://hub.docker.com/r/jupyter/all-spark-notebook and download the image if you don't know what an image is in docker no problem
you can see my repository on how to use and install docker and some useful tools to deploy your api.

The first thing is to open your docker desktop, then something like juypter/all-spark-notebokk appears
there you click on create<img src="https://i.stack.imgur.com/B2YO9.png" alt="Texto alternativo" width="300" height="200"> and something like this appears
Then in the part that says port put [8080](#id1),in Volume put the path whatever you want, and finally in container path put [/home/jovyan/work](#id2) 
and that is.
