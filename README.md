---
title: |
  PROSIT 2 Aller\
  Un conteneur dans les nuages
---

# Contexte

Léo veut mettre en place le logiciel GLPI mais Laila ne peut pas
installer de machine virtuelle sur son ordi, Marco propose d'utiliser
HyperV ou Docker.

# Mots clés

-   ITIL (Information Technology Infrastructure Library) : ITIL est un
    cadre de référence pour la gestion des services informatiques. Il
    propose des bonnes pratiques pour aligner les services IT sur les
    besoins des entreprises, en couvrant des domaines tels que la
    gestion des incidents, des changements et des niveaux de service.

-   Docker : Plateforme permettant de créer, déployer et exécuter des
    applications dans des conteneurs. Les conteneurs isolent les
    applications et leurs dépendances, assurant une portabilité accrue
    entre les environnements de développement, de test et de production.

-   Hyperviseur : Un hyperviseur est un logiciel permettant de créer et
    de gérer des machines virtuelles. Type 1 : Exécuté directement sur
    le matériel physique (ex. VMware ESXi, Microsoft Hyper-V) ; Type 2 :
    Fonctionne au-dessus d'un système d'exploitation hôte (ex.
    VirtualBox, VMware Workstation).

-   PoC (Proof of Concept) : Une preuve de concept est un prototype ou
    une démonstration visant à prouver la faisabilité ou l'efficacité
    d'une idée, d'un produit ou d'une technologie avant un développement
    à grande échelle.

-   ITSN (Information Technology Service Network) : Réseaux dédiés à la
    fourniture de services IT, souvent utilisés dans un contexte de
    gestion centralisée des services IT et de communication entre les
    équipes ou systèmes.

-   VDI (Virtual Desktop Infrastructure) : VDI permet d'héberger des
    environnements de bureau virtuels sur un serveur centralisé. Les
    utilisateurs accèdent à leurs bureaux via des clients légers ou à
    distance, offrant flexibilité et sécurité.

-   Baremetal : Serveur physique sans couche logicielle intermédiaire
    (comme un hyperviseur). Les applications ou systèmes d'exploitation
    sont installés directement sur le matériel.

-   Cluster (Hyper-V) : Ensemble de serveurs interconnectés qui
    travaillent ensemble pour assurer la disponibilité des machines
    virtuelles. Il offre des fonctionnalités comme la migration en
    direct et la tolérance aux pannes.

-   RDP (Remote Desktop Protocol) : Protocole de Microsoft permettant de
    se connecter à distance à un autre ordinateur via une interface
    graphique. Il est souvent utilisé pour administrer des serveurs ou
    des postes de travail à distance.

-   SSH (Secure Shell) : Protocole sécurisé permettant l'accès à
    distance à un serveur ou à un autre système informatique. Il offre
    des fonctionnalités telles que le transfert de fichiers et
    l'exécution de commandes sur des systèmes distants.

-   GLPI (Gestion Libre de Parc Informatique) : Application open-source
    de gestion des ressources IT. Elle propose des fonctionnalités pour
    gérer les inventaires, les tickets, la maintenance et les contrats.

-   Help desk : Service de support informatique fournissant une
    assistance aux utilisateurs pour résoudre des problèmes techniques
    ou répondre à des questions.

-   PHP (Hypertext Preprocessor) : Langage de programmation côté serveur
    largement utilisé pour développer des applications web. Il est
    notamment utilisé dans les systèmes de gestion de contenu comme
    WordPress et les applications personnalisées.

# Problématique

Comment déployer une solution ITSN/GLPI qui améliore la gestion actuelle
sous Excel en respectant les contraintes de virtualisation ?

# Contraintes

-   Pas de VirtualBox

-   GLPI: Serveur web Base de données

-   Pas de droits admin

# Livrables

-   GLPI déployé sur Docker/HyperV

-   Schéma d'architecture

-   Comparatif Docker/HyperV

-   Plan de déploiement

# Généralisations

-   Conteneurisation

-   Bonnes pratiques Git

-   Virtualisation

-   Serveur web

# Pistes de solutions

-   Comparatif : Consommation Facilité de déploiement

-   Utiliser les outils proposés par le logiciel pour l'installer

-   Suivre les recommandations d'installation du logiciel

# Plan d'action

1.  Analyser besoins d'installation GLPI

2.  Réfléchir aux étapes du déploiement

3.  Déployer GLPI sur Docker et HyperV

4.  Comparer

5.  Faire un guide de déploiement sur Docker et HyperV

# Réalisation

## Mathéo

Avec docker-compose: permet de structurer un \"docker run\" dans un
fichier. 2 containers: 1 pour la bdd, 1 pour GLPI. Transferable entre
n'importe quelle machine

## Grégoire et Thibault

Hyperviseur type 1 (Proxmox).\
Serveur Apache qui fait tourner GLPI.\
Instructions du site web GLPI. 
