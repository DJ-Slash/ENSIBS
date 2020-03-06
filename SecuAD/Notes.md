# Techniques pour pentest un Active Directory

### Introduction et termes
Afin de bien comprendre comment pentester un AD, il est nécessaire d'expliciter quelques termes :
- DC (Domain Controller) : Machine portant l'Active Directory

### But final
**Passer admin du domaine.**

### Première étape : Obtention d'un accès à l'AD
Il existe deux grands moyens pour obtenir un accès à l'AD :
- **Anonymous Bind** : Fonctionnalité permettant de se connecter à l'AD sans avoir de comptes
- **BruteForce d'un utilisateur**

Une fois connecté à l'AD, on va pouvoir passer à l'énumération.

### Deuxième étape : Enumération
Pour se faire, on peut utiliser différentes méthodes :
- En se connectant directement à l'AD : à l'aide de l'outil rpcclient, il est possible de se connecter directement à l'AD. On obtient alors une CLI permettant d'exécuter des commandes (lister les utilisateurs, les groupes,...)
> $ rpcclient <IP du DC> -U "" -N
- En utilisant le tool enum4linux


## Tools
- Bloodhound : TODO
- Crackmapexec : TODO
