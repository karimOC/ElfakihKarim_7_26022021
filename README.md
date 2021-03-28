
Backend :
Ce projet est développé avec NodeJS, Express, Sequelize et Mysql

Frontend :
Ce projet est développé avec VueJS

L'installation de NodeJS, Express, Sequelize et Mysql est requise sur votre ordinateur.

**FRONTEND**

Clônez le repo sur lequel vous vous trouvez.

À la racine du dossier frontend => npm install

Puis npm run serve

Vous verrez ensuite 2 urls: copier et coller l'url Network dans votre navigateur web.

(Exemple:
App running at:
  - Local:   http://localhost:8080/ 
  - Network: http://192.168.1.64:8080/)

**Installation de la base de données**
Entrez: - npm i sequelize
        - sequelize init

Dans le dossier backend modifer le mot de passe dans config/config.json

Créez une base de données nommée "groupomania" dans votre base de données mysql. Command : CREATE DATABASE groupomania;

Pour finaliser la base de données, executez dans la racine du dossier backend : Command : "sequelize db:migrate"

Puis lancez le serveur avec "npm start"

Pour modifier le mot de passe 

Installer le logiciel MAMP
Dans preférences/ports cliquez sur le ports 80 & 3306
Ensuite cliquez sur START

**BACKEND**

Installer mysql dans le backend => npm i mysql

À la racine du dossier backend, faites un npm install

Faites un node server ou nodemon server (node recquis pour cette aplication)

