![WealthHealth](WealthHealth.webp)


# OPENCLASSROOMS PROJECT 14 *(English)*

# Wealth Health

- THIS IS THE BACKEND NEEDED FOR THE WEALTH HEALTH PROJECT
- THE FRONTEND CAN BE FOUND AT BRANCH "db" [FrontEnd](https://github.com/Stevens-Mark/StevensMark_P14_04022022-)

## Switch a jQuery library to React

## Scenario
Wealth Health is a large financial company who uses an internal web application, called HRnet that manages employee records. The application is old and uses jQuery on the front end, which leads to considerable bugs and increased internal complaints. 
The biggest issues for HRnet users are date pickers, modal windows, drop down menus, and tables. Several complaints that the jQuery plugins are very slow have been received.
The company wants to create their own React components instead of these third-party jQuery plugins that are used in the user interface and hope that converting these jQuery plugins into React components will improve the performance and stability.  
As Management doesn't want this first part of the conversion process to take too long, pick ONE of the four jQuery plugins and convert it to a React component.

## Objective

### HRNet project conversion
-	The whole HRNet application has to be converted to React.
-	Make a new version of the "Create Employee" and "Employee List" pages with React.
-	Add a state management system (the current version uses local storage).
-	Make sure that everything is consistent in style. No need to redesign the application, but if so, change the style to something more modern.  
-	If time, test the React code with a unit test suite. Otherwise, only manual tests are needed. 

### Plugin conversion
Here is the list of currently used jQuery plugins that need to be converted: 
-	Date picker plugin
-	Modal window plugin - jQuery.modal.js
-	Drop down menus
-	Plugin for data tables

### Performance testing
-	The company wants to measure quantifiable data (e.g. page load times, network calls) to ensure that converting the app to React actually improves performance. To do this, do Lighthouse performance audits. To compare, do one for the current jQuery HRnet application, and then another once the application and the chosen jQuery plugin are converted to React.
-	Once the HRnet app in React is working, publish the React component to npm as a package and share the link it can used later if needed.

## Technical constraints
-	Follow a functional programming paradigm when writing these libraries in React.
-	Avoid using classes when you convert the old application. 
-	Write smaller, modular pieces of code and standalone functions for optimal modularity and maintainability. 
-	When converting a jQuery plugin to a React component, keep in mind to convert only the code that deals with the actual functionality of the plugin's user interface. For example, if you convert a jQuery plugin for a modal window, focus on creating a React component that works as a modal window, and nothing else.
-	Document the converted React component with a general description of what the component does and comments explaining what each accessory is for and how it is used.

## Here is a summary of the main tasks: 
- Convert the entire HRNet project to React. 
- Convert one of the four current jQuery plugins to React. Replace the 3 remaining jQuery plugins with React components. 
- Perform Lighthouse performance tests comparing the old and new application. 

## Skills
- [x] Redesign an application to reduce technical debt
- [x] Analyze the performance of a web application
- [x] Deploy a front-end application
- [x] Programming in JavaScript with functional programming

# Installation *(English)*

## Prerequisites
- [NodeJS](https://nodejs.org/en/)  Version 16.13.0 
- [NPM](https://www.npmjs.com/package/npm) Version 7.6.0
- [Visual Studio Code](https://code.visualstudio.com/) or another IDE of your choice

## Dependencies
- [Express](https://expressjs.com/) Version 4.17.3
- [Mongoose](https://www.npmjs.com/package/mongoose) Version 6.2.8

## Installing and running the project

### BackEnd

- Clone the repository P14_Backend onto your computer : 
  `git clone https://github.com/Stevens-Mark/P14_Backend.git`

- Inside this repository, install the packages/dependencies :
 `npm install`

### Create your own Database

- Create an account with [MongoDB](https://account.mongodb.com/account/login)
- Sign up for a free account. Once you have access to your dashboard, create a new cluster, and set it up with the AWS option and only free tier options to keep development free.
- Go to the Security tab. First, you'll want to add a new user with the ability to read and write to any database. You can choose any username and password, but write it down, as you will need it to connect your API to your cluster. The name of your cluster and/or database is unimportant but CALL THE COLLECTION "employees".

- You will also need to go to the IP Whitelist tab and add your current IP address (which you will need to update whenever it changes) or allow access from anywhere.

### How to connect your API to your MongoDB Cluster

-From your MongoDB Atlas, click the Connect button, and choose "Connect your application." You can then select "driver 3.6 or later" and COPY the generated SRV address as you will paste this in the app.js file.
- Go to the app.js file: at line 10: 
- mongoose.connect('mongodb+srv://<username>:<password>@cluster0.z3atg.mongodb.net/<database_name>?retryWrites=true&w=majority')
- Replace the SRV address with your own MongoDB <username> <password> <database_name> strings.
- To start your server type  `nodemon server`
- After saving this and restarting your server if necessary, you should see "Listeniing on port 3000, Successfully connected to MongoDB Atlas" logged to the console. Your API is now connected to your database cluster!!

- Once the server is running, install & run the FrontEnd.

- If you are having trouble & If the course still exists see: OpenClassrooms: 
- [Go Full-Stack With Node.js, Express, and MongoDB](https://openclassrooms.com/en/courses/5614116-go-full-stack-with-node-js-express-and-mongodb/5656211-set-up-your-database)

### FrontEnd
- Clone the repository onto your computer : branch "db"
  `git clone https://github.com/Stevens-Mark/StevensMark_P14_04022022-`

- Inside this repository, install the packages/dependencies :
 `npm install`

- Run the Api:
 `npm start`

The App runs on http://localhost:3001/


# OPENCLASSROOMS PROJECT 14 *(Fran??ais)*

# Wealth Health

- IL S'AGIT DU BACKEND N??CESSAIRE AU PROJET DE WEALTH HEALTH.
- LE FRONTEND PEUT ??TRE TROUV?? DANS LA BRANCHE "db" [FrontEnd](https://github.com/Stevens-Mark/StevensMark_P14_04022022-)


## Faites passer une librairie jQuery vers React

## Sc??nario
Wealth Health est une grande soci??t?? financi??re qui utilise une application web interne, appel??e HRnet, pour g??rer les dossiers des employ??s. L'application est ancienne et utilise jQuery sur le front-end, ce qui entra??ne des bogues consid??rables et une augmentation des plaintes internes. 
Les plus gros probl??mes pour les utilisateurs de HRnet sont les s??lecteurs de date, les fen??tres modales, les menus d??roulants et les tableaux. Plusieurs plaintes selon lesquelles les plugins jQuery sont tr??s lents ont ??t?? re??ues.
L'entreprise veut cr??er ses propres composants React au lieu de ces plugins jQuery tiers qui sont utilis??s dans l'interface utilisateur et esp??re que la conversion de ces plugins jQuery en composants React am??liorera les performances et la stabilit??.  
Comme la direction ne veut pas que cette premi??re partie du processus de conversion prenne trop de temps, choisissez UN des quatre plugins jQuery et convertissez-le en composant React.


## Objectif

### Conversion du projet HRNet 
- L'ensemble de l'application HRNet doit ??tre converti en React.
- Faire une nouvelle version des pages "Cr??er un employ??" et "Liste des employ??s" avec React.
- Ajouter un syst??me de gestion des ??tats (la version actuelle utilise le stockage local).
- Veillez ?? ce que tout soit coh??rent en termes de style. Pas besoin de redessiner l'application, mais si c'est le cas, changez le style pour quelque chose de plus moderne.  
- Si le temps le permet, testez le code React avec une suite de tests unitaires. Sinon, seuls des tests manuels sont n??cessaires. 


### Conversion des plugins
Voici la liste des plugins jQuery actuellement utilis??s qui doivent ??tre convertis : 
- Plugin de s??lection de date
- Plugin de fen??tre modale - jQuery.modal.js
- Menus d??roulants
- Plugin pour les tables de donn??es

### Tests de performance
- L'entreprise veut mesurer des donn??es quantifiables (par exemple, les temps de chargement des pages, les appels r??seau) pour s'assurer que la conversion de l'appli ?? React am??liore r??ellement les performances. Pour ce faire, effectuez des audits de performance Lighthouse. Pour comparer, faites-en un pour l'application HRnet actuelle en jQuery, puis un autre une fois que l'application et le plugin jQuery choisi sont convertis en React.
- Une fois que l'application HRnet en React fonctionne, publiez le composant React sur npm en tant que package et partagez le lien qui pourra ??tre utilis?? ult??rieurement si n??cessaire.


## Contraintes techniques
- Suivez un paradigme de programmation fonctionnelle lorsque vous ??crivez ces biblioth??ques en React.
- ??vitez d'utiliser des classes lorsque vous convertissez l'ancienne application. 
- ??crivez des morceaux de code plus petits et modulaires et des fonctions autonomes pour une modularit?? et une maintenabilit?? optimales. 
- Lorsque vous convertissez un plugin jQuery en composant React, gardez ?? l'esprit de ne convertir que le code qui traite de la fonctionnalit?? r??elle de l'interface utilisateur du plugin. Par exemple, si vous convertissez un plugin jQuery pour une fen??tre modale, concentrez-vous sur la cr??ation d'un composant React qui fonctionne comme une fen??tre modale, et rien d'autre.
- Documentez le composant React converti avec une description g??n??rale de ce que fait le composant et des commentaires expliquant ?? quoi sert chaque accessoire et comment il est utilis??.

## Voici un r??capitulatif des principales t??ches : 
- Convertir l'ensemble du projet HRNet en React. 
- Convertir l'un des quatre plugins jQuery actuels en React. Remplacer les 3 plugins jQuery restants par des composants React. 
- Effectuer des tests de performance Lighthouse en comparant l'ancienne et la nouvelle application. 

## Skills
- [x] Refondre une application pour r??duire la dette technique
- [x] Analyser la performance d'une application web
- [x] D??ployer une application front-end
- [x] Programmer en JavaScript avec la programmation fonctionnelle

# Installation *(fran??ais)*

## Pr??requis
- [NodeJS](https://nodejs.org/en/)  Version 16.13.0 
- [NPM](https://www.npmjs.com/package/npm) Version 7.6.0
- [Visual Studio Code](https://code.visualstudio.com/) ou un autre IDE de votre choix

## D??pendances
- [Express](https://expressjs.com/) Version 4.17.3
- [Mongoose](https://www.npmjs.com/package/mongoose) Version 6.2.8

## Installer et ex??cuter le projet

### BackEnd

- Clonez le d??p??t P14_Backend sur votre ordinateur : 
  `git clone https://github.com/Stevens-Mark/P14_Backend.git`

### Cr??er votre propre base de donn??es

- Cr??er un compte avec [MongoDB](https://account.mongodb.com/account/login)
- Cr??ez un compte gratuit. Une fois que vous avez acc??s ?? votre tableau de bord, cr??ez un nouveau cluster, et configurez-le avec l'option AWS et uniquement les options du niveau gratuit pour garder le d??veloppement gratuit.
- Allez dans l'onglet S??curit??. Tout d'abord, vous voudrez ajouter un nouvel utilisateur ayant la capacit?? de lire et d'??crire dans n'importe quelle base de donn??es. Vous pouvez choisir n'importe quel nom d'utilisateur et mot de passe, mais notez-le, car vous en aurez besoin pour connecter votre API ?? votre cluster. Le nom de votre cluster et/ou de votre base de donn??es n'a pas d'importance, mais appelez la collection "employees".

- Vous devrez ??galement aller dans l'onglet Liste blanche d'IP et ajouter votre adresse IP actuelle (que vous devrez mettre ?? jour chaque fois qu'elle change) ou autoriser l'acc??s depuis n'importe o??.

### Comment connecter votre API ?? votre cluster MongoDB

-Depuis votre Atlas MongoDB, cliquez sur le bouton Connecter, et choisissez "Connecter votre application". Vous pouvez ensuite s??lectionner "driver 3.6 ou plus" et COPIER l'adresse SRV g??n??r??e car vous allez la coller dans le fichier app.js.
- Allez dans le fichier app.js : ?? la ligne 10 : 
- mongoose.connect('mongodb+srv://<username>:<password>@cluster0.z3atg.mongodb.net/<database_name>?retryWrites=true&w=majority')
- Remplacez l'adresse SRV par vos propres cha??nes MongoDB <username> <password> <database_name>.
- Pour d??marrer votre serveur, tapez `nodemon server`.
- Apr??s avoir sauvegard?? et red??marr?? votre serveur si n??cessaire, vous devriez voir "Listeniing on port 3000, Successfully connected to MongoDB Atlas" enregistr?? dans la console. Votre API est maintenant connect??e ?? votre cluster de base de donn??es !

- Une fois le serveur en marche, installez et ex??cutez le FrontEnd.

- Si vous rencontrez des difficult??s et si le cours existe toujours, consultez : OpenClassrooms : 
- [Passez au Full Stack avec Node.js, Express et MongoDB](https://openclassrooms.com/en/courses/6390246-passez-au-full-stack-avec-node-js-express-et-mongodb/6466348-configurez-votre-base-de-donnees)


### FrontEnd
- Clonez le repo sur votre ordinateur :
  `git clone https://github.com/Stevens-Mark/StevensMark_P14_04022022-`

- Dans ce d??p??t, installez les paquets/d??pendances :
 `npm install`

- Ex??cutez l'Api :
 `npm start`

L'application fonctionne sur http://localhost:3001/
