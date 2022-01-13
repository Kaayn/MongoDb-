# MongoDb-


## Création d'un compte MongoDb!
[Creation de compte mongodb](https://user-images.githubusercontent.com/47184542/149176268-32e4594b-86f4-4344-b53c-7acf54d84ba3.png)

## Invitation sur le cluster créer par Rabire 
![image](https://user-images.githubusercontent.com/47184542/148751699-f300010c-4cbe-4bbc-8d5f-9bb78bd491e1.png)

## Création de la DataBase 
![image](https://user-images.githubusercontent.com/47184542/148751982-97f32eb7-98e6-4d81-a06b-68cb74dc2701.png)
![image](https://user-images.githubusercontent.com/47184542/148752731-201804c3-333f-42c0-9a65-562f6198aad0.png)
![image](https://user-images.githubusercontent.com/47184542/148752833-62ae3751-c605-419a-8a20-7304bf807290.png)

## Ajout d'un user root
![image](https://user-images.githubusercontent.com/47184542/148753384-6236cdb1-b924-480f-b6c8-c91e3b8a4ee2.png)

## Ajout de nos adresses IP
![image](https://user-images.githubusercontent.com/47184542/148753256-98541fd0-aa8c-4dd6-9e56-bbe91830a344.png)

## Essai de connexion avec MangoDB Shell
![image](https://user-images.githubusercontent.com/47184542/149177239-06bb338e-a55c-4ee3-b9e9-a7f5e5fa78a5.png)

On a eu des soucis avec Shell donc on est passé sur Compass

## Installation de Compass + Ajout de la table restaurants
![image](https://user-images.githubusercontent.com/47184542/148757618-515efc70-fed2-4500-86a5-72d9ae827b7e.png)

## Importation d'une table clients (1000 documents)
![image](https://user-images.githubusercontent.com/47184542/149178218-ec38ee6d-7134-4713-ad35-5987796125af.png)



## Compte rendu MongoDb

Dans notre projet l'utilisation d'un SGBD nous est uitle pour gerer nos restaurants et analyser nos clients.
C'est impératif d'avoir une base de donnée organisé avec de bonne performance. 
Pour créer une requete on regarde le besoin et on fais en fonction.

On a commencer par creer des fake datas Clients grace a ce site 
https://www.mockaroo.com/
On leurs a mis des geoDatas dans un array(Longitude/latitude), on a eu du mal a les mettres en place au début.

Chart est un execellent moyen de creer des graphique grace au donnees qu'on lui confie, savoir ou se situe le plus de traffic sur l'ensemble de nos restaurant, ou la ou le traffic est le moins présent. On peut donc affiner en fonction, creer plus de restaurant dans une certaine zone, faire du marketting ou bien meme de la pub dans les endroits ou le traffic est plus faible. L'idée derriere cette démarche est potentiellement de fidéliser un maximum de client. 

## Creation d'une chart grace au geoDatas 
![image](https://user-images.githubusercontent.com/47184542/148927876-7539b341-8f32-4c3e-80fc-622bebe473d3.png)

## Index 

L'index permet de se déplacer plus rapidement a travers toutes les collections, c'est un parti indépendante qui affiche nos données selon un tri par ordre

![image](https://user-images.githubusercontent.com/47184542/149181846-d3c866a2-ed50-42bb-81e9-3593d983375b.png)

J'ai pas trouvé d'endroit ou mettre un index qui soit utile, au départ je voulais `db.clients.createIndex(a:1, options, commitQuorum)`

## Requêtes d'aggrégation 

https://rtavenar.github.io/mongo_book/content/05_agreg.html

Les requêtes d'aggrégation permettent d'additionner, regrouper , compter des données. 

![image](https://user-images.githubusercontent.com/47184542/149180990-3e6e78ae-0d0a-4f3a-93a3-0ebf59c07f90.png)

Donc la mon but ca vas etre d'analyser nos clients, qui, quand et ou, pour après adapter nos restos a la demande et faire de la pub.

Dans la requete qui suis je prend un tranche d'age pour reorienté nos clients dans des restos qu'ils leurs correspondront le plus 

![image](https://user-images.githubusercontent.com/47184542/149364452-33a19dd7-73cb-4220-825f-b50bde25c0b7.png)

Donc la je connais la moyenne d'age de mes clients.

![image](https://user-images.githubusercontent.com/47184542/149344771-89294d63-82c3-46ad-95dc-7d907ef3a2a0.png)

J'ai aussi récupérer tout les e-mail de nos clients 

![image](https://user-images.githubusercontent.com/47184542/149344899-f0747e99-a2ff-4cde-99af-9714fee5c6b5.png)

Grace a cette requete j'ai une idée claire de quand et qui vient dans les restos 

![image](https://user-images.githubusercontent.com/47184542/149341194-8b7733a8-e326-4c57-87e8-5219d930eb70.png)

Exemple d'un objet JSON que je récupère 

![image](https://user-images.githubusercontent.com/47184542/149343615-184b0cce-b78e-48e6-9598-0c1a790f7fdc.png)

Je vois que Zeke est un client récurent et donc une personne à qui je vais pouvoir proposer des offres qu'il sera plus susceptible de prendre.



Question 1. Tout les documents
![image](https://user-images.githubusercontent.com/47184542/148758306-5bbb1029-47fe-4840-bede-c9ccd45aaf52.png)

Question 2. 
![image](https://user-images.githubusercontent.com/47184542/148758947-bd3d8f22-fecd-4208-b16a-b2c1c14e1c7f.png)

Question 3.
![image](https://user-images.githubusercontent.com/47184542/148759042-88b504c0-dd6b-4fe7-9948-e941f0887b30.png)

Question 4. 
![image](https://user-images.githubusercontent.com/47184542/148759738-4fa8236c-65f5-4fd6-9ca1-1191d9094a27.png)

Question 5. 
![image](https://user-images.githubusercontent.com/47184542/148759845-a54df9b3-79bd-46cd-9736-5cdffe8376d3.png)

Question 6. 
![image](https://user-images.githubusercontent.com/47184542/148760973-ee420fff-1e94-4ab0-aad8-a9b0b4eb4455.png)

Question 7. 
![image](https://user-images.githubusercontent.com/47184542/148761168-ce499bb6-49f2-4878-85ae-f5d83c3374b0.png)

Question 8.
![image](https://user-images.githubusercontent.com/47184542/148761709-478d9e6a-4084-41cd-a855-238efe3e1bf3.png)




