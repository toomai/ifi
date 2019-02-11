# ifi

## Système d'exploitation

|**OS**|**Pour**|**Contre**|
|------|--------|----------|
|Windows 10|Plus léger| Licence couteuse|
||Habitudes utilisateurs||
|Windows Server|Proche de la production|Plus lourd|
||Bonne capacités de virtualisation  (HyperV)|Licence encore plus couteuse|
|Ubuntu|Gratuit|Ubuntu|
||Simplicité d'utilisation||
||Support de la part de Cannonical||

## Environement de développement

### IDE

#### Visual Studio

|**Pour**|**Contre**|
|--------|----------|
|Tout est inclus|Très lourd: IIS, SQL Server Express|
|Plug&Play| Licences assez chères (OS + VS)|
|Proche de la prod||
|Tout est centralisé||
|Métrique système||
|Intégration VCS||
|Console||
|Débugger||
|Éditeur de DB||
|Éditeur d'IHM (web ou pas) ||
|Intégration dans l'environnement Windows||

![Visual Studio](visualstudio.png)
![Visual Studio](visualstudio2.png)

#### Visual Studio Community

|**Pour**|**Contre**|
|--------|----------|
|Très similaire à la version Pro/Ent|Quelques fonctionnalités en moins|
|Suffisant pour une petite équipe||

#### Visual Studio Code

|**Pour**|**Contre**|
|--------|----------|
|Léger|Très bas niveau|
|Gratuit|Plus technique que "Pousser sur le bouton vert"|
||Pas d'intégration poussée des technologies ASP (Edition de formulaire, DB)|

![Visual studio code](vsc1.png)
#### Mono

|**Pour**|**Contre**|
|--------|----------|
|Tourne sous Linux|Demande plus de paramétrage|
|Économie de coût|Installation d'un serveur en plus de l'IDE|
|Linux: Plus simple pour faire du déploiement automatisé (Ansible,...)||
|Plus compliqué de faire du développement orienté Windows (Client lourd)||

#### JetBrains Rider

* Pas réussi à le faire fonctionner

### Choix

Mon choix se porterait vers Windows pour le système d'exploitation. En effet si on veut éviter toutes les configurations pour "émuler" les librairies nécessaires pour Windows. On peut prendre Windows 10 (Pro) pour la simplicité d'utilisation et la familiarité des utilisateurs. Le second choix serait Windows Server, celui-ci offre de bonne capacité de configuration automatisée et est plus proche de l'environnement de production. Il offre aussi de bonnes capacités de virtualisations, ce qui est très bien dans un monde de micro-services dominé par des K8S et autres, il est possible de créer des machines paravirtuelles pour déploier des environnements complets. Il est cependant plus lourd à déploier et parfois plus compliqué à prendre en main.

Au niveau de l'IDE, je choisirais Visual Studio Community ou Pro/Entreprise. En effet, les deux IDE se démarquent fortement par rapport aux autres au niveau de leur intégration dans l'environnement Windows. Si on se cantonne à faire du  Web les autres solutions sont très bien. Cependant dès que l'on veut faire du développement orienté Windows, il est plus simple de partir sur cette solution. Finalement il est supporté par l'éditeur du langage le rendant plus adapté.
