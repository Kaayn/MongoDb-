# MongoDb-
Cours 10/01/2022

Création d'un compte MongoDb

Invitation sur le cluster créer par Rabire 
![image](https://user-images.githubusercontent.com/47184542/148751699-f300010c-4cbe-4bbc-8d5f-9bb78bd491e1.png)

Création de la DataBase 
![image](https://user-images.githubusercontent.com/47184542/148751982-97f32eb7-98e6-4d81-a06b-68cb74dc2701.png)
![image](https://user-images.githubusercontent.com/47184542/148752731-201804c3-333f-42c0-9a65-562f6198aad0.png)
![image](https://user-images.githubusercontent.com/47184542/148752833-62ae3751-c605-419a-8a20-7304bf807290.png)

Création d'un user root
![image](https://user-images.githubusercontent.com/47184542/148753384-6236cdb1-b924-480f-b6c8-c91e3b8a4ee2.png)

Ajout de nos adresses IP
![image](https://user-images.githubusercontent.com/47184542/148753256-98541fd0-aa8c-4dd6-9e56-bbe91830a344.png)

Installation de Compass + Ajout du JSON restaurant
![image](https://user-images.githubusercontent.com/47184542/148757618-515efc70-fed2-4500-86a5-72d9ae827b7e.png)

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


Compte rendu MongoDb

Dans notre projet l'utilisation d'un SGBD nous est uitle pour gerer nos restaurants et analyser nos clients.
C'est impératif d'avoir une base de donnée organisé et avec de bonne performance. 
Pour créer une requete on regarde le besoin et on fais en fonction, par exemple pour savoir d'ou vienne nos clients on calcule leur position grace a leur geoData.

On a creer des fake datas Clients grace a ce site 
https://www.mockaroo.com/
On leurs a mis des geoDatas dans un array(Longitude/latitude), on a eu du mal a les mettres en place au début.

Chart est un execellent moyen de creer des graphique grace au donnees quon lui confie, savoir ou se situe le plus de traffic sur l'ensemble de nos restaurant, ou la ou le traffic est le moins présent. On peut donc affiner en fonction, creer plus de restaurant dans une certaine zone, faire du marketting ou bien meme de la pub dans les endroits ou le traffic est plus faible. L'idée derriere cette démarche est potentiellement de fidéliser un maximum de client. 

Creation d'une chart grace au geoDatas ![image](https://user-images.githubusercontent.com/47184542/148927876-7539b341-8f32-4c3e-80fc-622bebe473d3.png)





