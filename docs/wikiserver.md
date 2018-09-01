# Wiki Server

## Hardware

Qualsiasi macchina va bene. Testato su un pc 32 bit. Ma dovrebbe funzionare benissimo anche su Raspberry PI.

## Software

- installare ubuntu server o raspbian
- ```sudo apt-get update```
- ```sudo apt-get upgrade -y```
- ```sudo apt-get install nginx supervisor -y```
- ```sudo apt-get install postgresql postgresql-contrib -y```
- clonare il repo wikidatabase
- ```sudo -i -u postgres```
- ```psql < wiki.sql```
- ```psql -d wiki``` ( controllare che il comando precedente sia andato a buon fine )
- ```exit```
- ```sudo add-apt-repository -y ppa:webupd8team/java```
- ```sudo apt-get update```.
- ```sudo apt-get install -y oracle-java8-installer``` ( seguire l installazione perchè chiederà alcune informazioni )
- clonare il repo wikiserver.
- ```./gradlew clean stage```.
- configurare nginx e supervisor.