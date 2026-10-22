# Sécurisation des accès réseau — CNTE

> Projet de fin d’études réalisé au Centre National des Technologies de l’Éducation (CNTE), dans le cadre de la sécurisation et de l’administration des accès réseau.

## Présentation

Ce projet porte sur la conception et la mise en œuvre d’une solution combinant l’authentification centralisée des utilisateurs et l’application de politiques de sécurité réseau. L’objectif est de mieux contrôler l’accès aux réseaux filaires et Wi-Fi et de renforcer la navigation web dans un contexte éducatif.

## Objectifs

- Centraliser la gestion des identités et des comptes utilisateurs avec OpenLDAP.
- Mettre en place l’authentification réseau à l’aide de FreeRADIUS et du standard IEEE 802.1X.
- Préparer la segmentation du réseau avec des VLAN et une topologie réseau simulée.
- Configurer une politique de filtrage d’URL au moyen de Cisco SD-WAN.
- Vérifier le fonctionnement à l’aide de tests d’authentification et de filtrage.

## Architecture et technologies

- **OpenLDAP** : annuaire centralisé des utilisateurs.
- **FreeRADIUS** : service d’authentification réseau.
- **IEEE 802.1X** : contrôle d’accès au réseau filaire et Wi-Fi.
- **DaloRADIUS** : interface web de gestion et de suivi de RADIUS.
- **LDAP Account Manager (LAM)** : interface d’administration de l’annuaire LDAP.
- **MariaDB** : base de données utilisée par la solution RADIUS.
- **Cisco SD-WAN** : politiques de sécurité et filtrage d’URL.
- **Huawei eNSP** : simulation de la topologie réseau et configuration des VLAN.
- **MobaXterm / Linux** : administration distante et configuration des services.

## Travaux réalisés

1. Étude de l’architecture réseau et conception de la solution proposée.
2. Simulation de la topologie réseau et préparation de la segmentation par VLAN.
3. Installation et configuration des composants FreeRADIUS, OpenLDAP, DaloRADIUS et LAM.
4. Intégration de l’annuaire LDAP avec FreeRADIUS.
5. Préparation de l’authentification réseau avec 802.1X pour les accès filaires et Wi-Fi.
6. Configuration d’une politique de filtrage d’URL dans Cisco SD-WAN, avec règles par catégories et listes d’URL.
7. Réalisation de tests pour vérifier les authentifications et le comportement du filtrage.

## Validation

Le rapport documente notamment :

- des tests de connectivité dans la topologie simulée ;
- un test d’authentification RADIUS/LDAP ;
- des scénarios d’accès avec différents profils d’utilisateurs ;
- des tests de filtrage d’URL et de blocage.

Les captures de ce dépôt doivent illustrer des résultats réellement observés dans le cadre du projet. Les environnements simulé et réel doivent être distingués clairement dans les légendes.

## Captures du portfolio

Tu peux ajouter dans le dossier `images/` des captures nettoyées et lisibles, par exemple :

- `architecture-solution.png` — architecture générale de la solution ;
- `topologie-ensp.png` — topologie réseau simulée ;
- `test-radius-ldap.png` — preuve de test d’authentification ;
- `politique-filtrage-sdwan.png` — configuration de la politique de filtrage ;
- `validation-filtrage.png` — résultat de validation du filtrage.

N’ajoute que les images que tu es autorisée à publier et qui ne révèlent aucune information confidentielle.

## Confidentialité et sécurité

Le rapport de stage peut contenir des identifiants, mots de passe d’exemple, adresses IP, noms d’équipements ou détails internes. **Ne publie pas ces informations dans un dépôt public.** Avant d’ajouter une capture :

- masque les mots de passe, secrets partagés, clés, jetons et identifiants ;
- masque les adresses IP internes et les informations permettant d’identifier l’infrastructure du CNTE, si elles ne sont pas autorisées à être diffusées ;
- retire les noms de comptes et toute donnée personnelle ;
- vérifie que le CNTE autorise la publication des captures et des détails de configuration ;
- ne publie pas le rapport PDF complet sans autorisation explicite.

Les valeurs d’identification et mots de passe présents dans le rapport ne doivent jamais être repris dans ce README ni dans les captures publiques.

## Périmètre du projet

Ce dépôt présente une synthèse pédagogique du projet de fin d’études. Il ne contient pas de configuration opérationnelle, de secrets, ni de données internes de l’organisation.

## Auteur

**Ranim Mili** — Projet de fin d’études en réseaux et cybersécurité.

