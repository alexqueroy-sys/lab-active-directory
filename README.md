# 🏰 Lab Active Directory — Windows Server 2022

## 📋 Description
Mise en place d'un environnement Active Directory complet en lab 
virtuel sous VirtualBox, simulant une infrastructure d'entreprise.

## 🏗️ Architecture
| Machine | OS | Rôle | IP |
|---|---|---|---|
| SRV-AD01 | Windows Server 2022 | Contrôleur de domaine | 192.168.10.1 |
| CLIENT-01 | Windows 10 Pro | Poste utilisateur | 192.168.10.10 |

## ✅ Ce qui a été configuré
- Promotion du serveur en contrôleur de domaine (AD DS)
- Configuration DNS et DHCP
- Création d'une structure OU (Direction, Informatique, Comptabilité)
- Création d'utilisateurs et groupes (GRP_IT, GRP_COMPTA)
- GPO : politique de mots de passe, restrictions panneau de configuration
- Jonction du poste Windows 10 au domaine lab.local
- Vérification des GPO avec gpresult /r

## 🛠️ Technologies utilisées
- Windows Server 2022
- Active Directory Domain Services (AD DS)
- VirtualBox 7.x
- PowerShell

## 📸 Screenshots

### Création VM Windows Server
![VM](Création%20VM%20Windows%20Server.PNG)

### Installation AD DS
![AD DS](Création%20AD%20DS.PNG)

### Création des groupes AD
![Groupes](Création%20groupes%20AD.PNG)

### GPO Mot de passe
![GPO MDP](GPO%20mdp.PNG)

### GPO Restrictions
![GPO Restriction](GPO%20Restriction.PNG)

### Connexion avec p.martin
![Connexion](Bien%20connecter%20avec%20P.MARTIN.PNG)

### GPO appliquées (gpresult)
![GPResult](LES%20GPO%20MARCHENT%20BIEN.PNG)

## 📚 Ce que j'ai appris
- Comprendre le rôle central d'AD en entreprise
- Gérer des utilisateurs et des droits d'accès
- Appliquer des politiques de sécurité via GPO
- Diagnostiquer des problèmes de jonction au domaine
