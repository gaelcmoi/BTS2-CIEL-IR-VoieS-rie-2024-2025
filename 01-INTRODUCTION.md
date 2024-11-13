# Les liaisons séries - Introduction

## Qu'est-ce que la voie série ?

La voie série est un protocole de communication où les données sont envoyées une à une, comme des perles enfilées sur un fil. Contrairement à la voie parallèle, où plusieurs bits de données sont envoyés en même temps sur des fils différents, la voie série utilise un seul fil pour transmettre tout le message, bit par bit. Parmi les exemples de communication série, on trouve des protocoles comme l'UART (Universal Asynchronous Receiver-Transmitter) ou l'I2C (Inter-Integrated Circuit), qui sont largement utilisés pour les communications entre microcontrôleurs et périphériques. À l'inverse, des protocoles comme le PCI (Peripheral Component Interconnect) ou le SCSI (Small Computer System Interface) sont basés sur la communication parallèle, envoyant plusieurs bits en même temps pour des transferts plus rapides mais nécessitant plus de lignes de câblage.

## Mais d'où ça vient, tout ça ?

L'idée de la communication en série remonte aux années 1960, avec l'invention de la norme RS-232 (Recommended Standard 232) par l'association EIA (Electronic Industries Association). Cette norme, conçue pour faciliter la communication entre les ordinateurs et leurs périphériques. À l'époque, les ordinateurs étaient énormes et les câbles très coûteux, ce qui rendait la voie série particulièrement intéressante pour économiser du matériel. Les premiers ordinateurs militaires et scientifiques ont ainsi rapidement adopté cette méthode pour permettre la communication entre différents composants tout en minimisant le nombre de fils nécessaires.

## Comment ça marche ?

La communication en voie série fonctionne en envoyant les données bit par bit sur une seule ligne de transmission. Chaque bit est transmis sous forme de signal électrique qui peut être haut (1) ou bas (0). Pour que les deux dispositifs se comprennent, ils doivent être synchronisés, c’est-à-dire qu'ils doivent s'accorder sur la vitesse à laquelle les bits sont envoyés, appelée "baud rate". Par exemple, un baud rate de 9600 signifie que 9600 bits sont transmis chaque seconde.

La communication série peut être soit asynchrone, soit synchrone. Dans le mode asynchrone, chaque octet de données est encadré par des bits de démarrage et d'arrêt, qui indiquent le début et la fin de la transmission d'un octet. Cela permet aux dispositifs de se synchroniser dynamiquement au début de chaque transmission, mais peut ajouter une certaine surcharge.

En mode synchrone, une horloge partagée est utilisée pour synchroniser l'envoi des bits, ce qui permet d'éliminer les bits de démarrage et d'arrêt et d'augmenter l'efficacité de la communication. Ce type de communication est souvent utilisé dans des systèmes où la rapidité et la précision sont cruciales, comme dans les systèmes embarqués ou les réseaux de capteurs industriels.

En résumé, la communication série est un processus méthodique où chaque bit est soigneusement transmis et interprété, assurant une communication claire et précise entre les dispositifs électroniques.

## Pourquoi c'est utile ?

La voie série est essentielle dans de nombreux domaines, y compris les environnements industriels. Par exemple, dans l'automatisation industrielle, des protocoles comme le Modbus RTU (Remote Terminal Unit) utilisent la communication série pour permettre aux automates programmables de contrôler des machines et des équipements à distance. Les réseaux de capteurs dans les usines, qui surveillent des paramètres comme la température ou la pression, utilisent souvent la communication série pour envoyer ces données à un contrôleur central. De plus, la voie série est couramment utilisée pour connecter des dispositifs de mesure, comme des débitmètres ou des variateurs de vitesse, à des systèmes de contrôle industriels, permettant une gestion précise et en temps réel des processus de production. Ces applications montrent à quel point la voie série est cruciale pour assurer une communication fiable et efficace dans les systèmes complexes.

En somme, la voie série est comme une ligne de communication discrète mais efficace, permettant aux appareils de "parler" entre eux, un bit à la fois. Et même si c'est plus lent qu'une autoroute de bits en parallèle, c'est souvent suffisant et bien plus pratique dans bien des cas.

Dans la prochaine partie du cours, nous allons voir une des normes les plus courantes pour les communciations en série : [la norme RS-232](Norme%20RS-232.md).
