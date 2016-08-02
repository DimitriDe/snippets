#NodeJS AngularJS Installation et ressources

##Packages à télécharger

**NodeJS**  
est un interpreteur JS "coté serveur"  
Télécharger : https://nodejs.org/dist/v6.3.1/node-v6.3.1-x64.msi

**Git**  
est pratique pour son client ainsi que GitBash qui va nous permettre d'avoir un environnement console comme Linux  
Télécharger : https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe

**Ruby**  
Utilisé par SASS  
Télécharger : http://dl.bintray.com/oneclick/rubyinstaller/rubyinstaller-2.3.1-x64.exe

**Github Desktop client**  
permet de cloner un projet, effectuer toutes les tâches : commit, push, pull, etc de manière visuelle  
Télécharger : https://github-windows.s3.amazonaws.com/GitHubSetup.exe

**Atom**  
est un éditeur pour le coding, il dispose de plugins puissants et d'un gestionnaire de projets  
Télécharger : https://atom.io/download/windows  
Plugins recommandés : Pigments, Minimap, File-icons

##Installer des modules complémentaires

Toutes ces commandes sont a lancer dans "Git Bash", il est recommandé de n'utiliser que lui comme terminal sous windows.

**Bower**  
Gestionnaire de paquets d'assets et de dépendances  
`npm install -g bower`

**Yeoman**  
Automatiser la création d'un projet et l'obtention de ses assets  
`npm install -g yo`

**Grunt**  
Effectuer des tâches automatisées récurentes  
`npm install -g grunt-cli`

**Live-server**  
Serveur web miniature qui permet de servir des fichiers statiques localement et gérer le live-reload
`npm install -g live-server`  
Pour lancer le serveur il suffit de taper : `live-server` dans un terminal au niveau du dossier que l'on veut partager

**SASS**  
"Compilateur" de fichiers CSS  
`gem install sass`

##Se lancer dans un projet existant

Si vous venez d'obtenir un projet via un clone, il est fort possible qu'il ne contienne aucune de ses dépendances.  
Ouvrez un GitBash et déplacez vous à la racine du projet puis tapez successivement : `npm install` et `bower install`

npm et bower utilisent chacun un fichier présent à la racine du projet qui leur indique quelles dépendances télécharger.  
package.json pour npm (node package manager)  
bower.json pour.. bower

##Tutoriaux et ressources sur AngularJS

**Formation AngularJS (Graphikart)**  
Introduction : https://www.grafikart.fr/formations/angularjs  
Les directives : https://www.grafikart.fr/formations/angularjs/directives  
Les controlleurs et le scope : https://www.grafikart.fr/formations/angularjs/controller-scope  
Les modules : https://www.grafikart.fr/formations/angularjs/module  
Les routes : https://www.grafikart.fr/formations/angularjs/routes  
Les services : https://www.grafikart.fr/formations/angularjs/services  
Les promesses : https://www.grafikart.fr/formations/angularjs/promesses  
Les filtres : https://www.grafikart.fr/formations/angularjs/filtres 

Créer des directives : https://www.grafikart.fr/formations/angularjs/creer-directive  
Les ressources : https://www.grafikart.fr/formations/angularjs/resources  
$apply, $watch, $digest : https://www.grafikart.fr/formations/angularjs/apply-watch-digest

**Autres**  
Tutoriels en français aussi : http://www.tutoriel-angularjs.fr/  
Blog sur Angular : http://www.frangular.com/

**Utiles**  
Récursion dans un template : http://jsfiddle.net/brendanowen/uXbn6/8/  
Promises : http://www.frangular.com/2012/12/api-promise-angularjs.html

**Composants**  
vAccordion : http://codepen.io/LukaszWatroba/pen/MwdaLo
