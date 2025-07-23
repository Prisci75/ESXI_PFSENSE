# ESXI_PFSENSE
TP sur ESXI et PFSENSE

**Déploiement d’une infrastructure réseau avec ESXi & pfSense**

Ce projet collectif vise à déployer une infrastructure réseau virtuelle complète de type Hub and Spoke, en s’appuyant sur la virtualisation imbriquée et la technologie VMware ESXi. L'architecture est renforcée par pfSense en tant que pare-feu central.


**Objectifs du projet :**


**1. Découvrir et utiliser la virtualisation imbriquée**

- Comprendre les cas d’usage : test, formation, isolation, rapidité de déploiement.
- Appliquer le concept via un hyperviseur de type 1 (VMware ESXi).


**2. Installer et configurer VMware ESXi**

- Création d’un compte VMware, téléchargement et installation d’ESXi v8.
- Ajout de disque, configuration du BIOS pour activer la virtualisation (Intel VT-x).


**3. Déployer une architecture en étoile avec pfSense comme routeur/pare-feu**

- Mise en place de pfSense comme nœud central pour gérer le trafic.
- Configuration WAN/LAN et création de règles de pare-feu.


**4. Créer plusieurs machines virtuelles spécialisées**

- VM Admin (Debian 12) : gestion, SSH, Ansible, DNS, Netdata.
- VM Wordpress (Debian 11) : déploiement via Ansible, pare-feu, HTTPS.
- VM Domaine AD (Windows Server 2016) : rôle DNS + Active Directory.
- VM Contrôleur de domaine : Domaine metsys.lan, supervision.


**5. Automatiser avec Ansible**

- Déploiement d’outils et services entre les VM via playbooks.


**6. Superviser l’infrastructure avec Netdata**

- Surveillance en temps réel des performances sur Linux et Windows.


**7. Configurer le réseau virtuel**

- Ajout de commutateurs, création de cartes réseau LAN sur toutes les VM.
- Connexion logique à pfSense pour un routage complet entre VM.


**Conclusion**

**Ce TP a permis d’appréhender les avantages d’un hyperviseur de type 1 (ESXi) :**

- Robustesse et sécurité accrues
- Optimisation matérielle
- Centralisation de la gestion réseau et services
- Réduction des coûts et de l’énergie


