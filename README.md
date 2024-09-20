 ### **Introduction** 
 
 Bonjour Soufiane, aujourd’hui je vais vous présenter le concept du projet **Menu Maker by Qwenta**
 
 --- ### **1. Présentation des livrables (15 minutes)** 
 
 #### **Contexte du projet** 
 Le projet **Menu Maker by Qwenta** est actuellement à l’étape de conception. Il s'agit d'une application web destinée à permettre aux restaurateurs de créer, personnaliser et gérer leurs menus en ligne. L'objectif principal est de simplifier la gestion des menus via une interface intuitive et réactive, tout en offrant des intégrations avec des plateformes de livraison telles que **Deliveroo** [oai_citation:15,Présentaton.pdf](file-service://file-8IN3fXiilWwOQugYoQ7x4apE). Nous avons réfléchi à un projet qui pourrait répondre aux besoins des restaurateurs en matière de flexibilité et de personnalisation, notamment en permettant des modifications en temps réel des menus et une gestion optimisée des prix et du branding [oai_citation:14,Menu Maker by Qwenta 0ffb7a8cab42800c9503f747d42b3f8e.pdf](file-service://file-9ktcMiHYOJBqEXJGD8GyliBp). 
 
 #### **Aperçu de la maquette** Nous avons conceptualisé une **maquette** qui pourrait présenter une interface simple, où les restaurateurs pourront créer et organiser des catégories de plats, modifier leurs menus en temps réel et gérer leurs tarifs de manière dynamique [oai_citation:13,Présentaton.pdf](file-service://file-8IN3fXiilWwOQugYoQ7x4apE). Les fonctionnalités imaginées incluent une interface de **glisser-déposer** pour faciliter la gestion des plats et des options de personnalisation visuelle [oai_citation:12,Menu Maker by Qwenta 0ffb7a8cab42800c9503f747d42b3f8e.pdf](file-service://file-9ktcMiHYOJBqEXJGD8GyliBp). 
 
 #### **Méthodologie envisagée** 
 Pour valider le passage d'une étape à une autre, nous suivrons une méthodologie **Agile**, avec des **sprints** de deux semaines. Chaque sprint commencera par une **planification**, suivie du développement, et se terminera par une **rétrospective** pour faire le point sur les tâches effectuées et ajuster la suite du projet en fonction des retours. Cela permet des livraisons régulières et une validation constante de l’avancement [oai_citation:11,Présentaton.pdf](file-service://file-8IN3fXiilWwOQugYoQ7x4apE). Pour valider le code, nous utiliserons un système de **branches GitHub**. Chaque développeur travaillera sur sa propre branche, et avant la fusion avec la branche principale, une **pull request** sera soumise pour une révision par un autre développeur. Cela garantit une validation par **code review**.
 
 #### **Gestion des User Stories et Story Points** 
 
 Chaque **User Story** correspond à une fonctionnalité ou un besoin exprimé par le restaurateur. Pour chaque User Story, nous utilisons un système de **Story Points** pour évaluer la complexité et l'effort nécessaire.
 
 #### **Planning Poker** 
 
 Pour estimer la complexité des tâches, nous utiliserons la technique du **Planning Poker**. Cette méthode de vote simultané permet à chaque membre de l'équipe de donner une estimation sans être influencé par les autres. En cas de divergence, une discussion permet d'atteindre un consensus, garantissant une meilleure estimation du temps nécessaire pour chaque tâche [oai_citation:8,Présentaton.pdf](file-service://file-8IN3fXiilWwOQugYoQ7x4apE). 
 
 #### **Méthode MoSCoW** 
 
Nous appliquerons également la méthode **MoSCoW** pour hiérarchiser les fonctionnalités : 
- **Must Have** : Fonctionnalités essentielles, comme la création de menus et l'authentification sécurisée via Firebase.
- - **Should Have** : Intégration de Deliveroo.
  - - **Could Have** : Ajout d’animations pour améliorer l’expérience utilisateur.
  - - **Won't Have** : Fonctionnalités non prioritaires, comme une version mobile complète dans la version initiale [oai_citation:7,Présentaton.pdf](file-service://file-8IN3fXiilWwOQugYoQ7x4apE). 

#### **Spécifications techniques prévues** 

Pour la partie technique, nous avons envisagé l’utilisation des technologies suivantes : 
- **Front-end** : Nous avons choisi **React.js** pour concevoir l’interface utilisateur, car il permet de créer des composants modulaires et réactifs. Le **SCSS** sera utilisé pour styliser l’application de manière flexible [oai_citation:6,spécification technique.pdf](file-service://file-1nTbGSoo0YhiLIAr3h43LVuj).
- - **Back-end** : Nous utiliserons **Node.js** et **Express.js** en combinaison avec **Firebase**. Le choix de **Firebase** plutôt que **MongoDB** repose sur plusieurs avantages clés adaptés aux besoins de notre projet. **Firebase** offre un écosystème complet et intégré qui gère non seulement la base de données en temps réel, mais aussi l’authentification des utilisateurs, l’hébergement, et la gestion de la sécurité via **Firebase Authentication** et **Firebase Security Rules**. Cela simplifie le développement en centralisant plusieurs services en une seule plateforme, réduisant ainsi la complexité technique. De plus, **Firebase** est optimisé pour les applications nécessitant des **mises à jour en temps réel**, une fonctionnalité essentielle pour permettre aux restaurateurs de modifier leurs menus et de voir les changements instantanément. Enfin, **Firebase** offre une **scalabilité automatique** et un modèle de tarification flexible basé sur l’usage, ce qui le rend particulièrement avantageux pour un projet en phase de lancement, où nous voulons minimiser les coûts tout en garantissant une infrastructure évolutive [oai_citation:5,spécification technique.pdf](file-service://file-1nTbGSoo0YhiLIAr3h43LVuj).


#### **Gestion des rôles et permissions** 

Pour la gestion des rôles et permissions, **Firebase Authentication** sera utilisé pour attribuer des rôles spécifiques aux utilisateurs, comme **restaurateurs** ou **administrateurs**. En fonction de ces rôles, nous appliquerons des **Firebase Security Rules** afin de restreindre l’accès à certaines sections de l’application. Par exemple, seuls les administrateurs pourront gérer les commandes, tandis que les restaurateurs pourront modifier uniquement leurs propres menus. Cette gestion fine des permissions nous permet d'assurer que les utilisateurs accèdent uniquement aux fonctionnalités auxquelles ils sont autorisés, renforçant ainsi la sécurité du projet [oai_citation:4,spécification technique.pdf](file-service://file-1nTbGSoo0YhiLIAr3h43LVuj). 

#### **Tests unitaires avec Jest** 

Pour soutenir cet argument, nous allons mettre en place des **tests unitaires** avec **Jest**. Jest est un framework de tests JavaScript qui nous permet de vérifier que chaque composant de l’application fonctionne correctement de manière isolée. Par exemple, pour le front-end, nous testerons les composants React afin de s'assurer qu'ils se comportent comme prévu, et que les états sont bien gérés. Nous testerons également la logique métier et les appels aux APIs pour garantir la cohérence des données. Ces tests seront exécutés automatiquement à chaque cycle de développement, avant chaque déploiement, pour s'assurer qu'aucune régression ne survient après des modifications [oai_citation:3,spécification technique.pdf](file-service://file-1nTbGSoo0YhiLIAr3h43LVuj). 

#### **Sécurité** 
Bien que notre équipe ne compte pas d’experts en cybersécurité, nous avons pris en compte plusieurs aspects de sécurité. Nous utiliserons **Firebase Authentication** pour gérer les sessions utilisateurs de manière sécurisée, et **Firebase Security Rules** pour contrôler l'accès aux données. Les en-têtes HTTP seront renforcés grâce à **Helmet.js**, et nous avons activé **HTTPS** par défaut via **Firebase Hosting**, garantissant ainsi une communication sécurisée entre le client et le serveur [oai_citation:2,spécification technique.pdf](file-service://file-1nTbGSoo0YhiLIAr3h43LVuj). 

### **2. Effectif de l’équipe** 

L’équipe envisagée pour ce projet est composée de plusieurs membres aux compétences complémentaires : 

- **Développeur Front-end** : Chargé de l’interface utilisateur en **React.js** et **SCSS**.
- - **Développeur Back-end** : Responsable de la gestion des données et de l'API via **Node.js**, **Express**, et **Firebase**.
  - - **Lead développeur** : Superviseur technique, qui s’assure de la cohésion entre le front-end et le back-end.
    - - **Testeur QA (partiel)** : Optionnel mais avantageux pour renforcer la qualité du produit via des tests fonctionnels.
      - - **Product Owner** : Gère les priorités et la communication avec les parties prenantes [oai_citation:1,Présentaton.pdf](file-service://file-8IN3fXiilWwOQugYoQ7x4apE).
          
#### **Testeur QA : Optionnel mais avantageux**
        Le rôle de **testeur QA** dans notre équipe est optionnel. En effet, grâce aux outils modernes comme **Jest** pour les tests unitaires et à des processus de tests automatisés, nous pouvons garantir un niveau de qualité suffisant sans avoir un testeur QA dédié à plein temps. Cependant, l'ajout d'un **testeur QA** pourrait représenter un atout significatif. En ayant une personne spécifiquement dédiée aux tests fonctionnels et à l’intégration, cela permettrait de repérer plus rapidement les bugs avant la livraison et d’assurer une qualité globale plus élevée du produit. Le testeur QA pourrait également superviser la bonne mise en place des critères d'acceptation définis dans les User Stories.

#### **Tests unitaires avec Jest** 

Pour soutenir cet argument, nous allons mettre en place des **tests unitaires** avec **Jest**. Jest est un framework de tests JavaScript qui nous permet de vérifier que chaque composant de l’application fonctionne correctement de manière isolée. Par exemple, pour le front-end, nous testerons les composants React afin de s'assurer qu'ils se comportent comme prévu, et que les états sont bien gérés. Nous testerons également la logique métier et les appels aux APIs pour garantir la cohérence des données. Ces tests seront exécutés automatiquement à chaque cycle de développement, avant chaque déploiement, pour s'assurer qu'aucune régression ne survient après des modifications [oai_citation:3,spécification technique.pdf](file-service://file-1nTbGSoo0YhiLIAr3h43LVuj). 

#### **Sécurité** 
Bien que notre équipe ne compte pas d’experts en cybersécurité, nous avons pris en compte plusieurs aspects de sécurité. Nous utiliserons **Firebase Authentication** pour gérer les sessions utilisateurs de manière sécurisée, et **Firebase Security Rules** pour contrôler l'accès aux données. Les en-têtes HTTP seront renforcés grâce à **Helmet.js**, et nous avons activé **HTTPS** par défaut via **Firebase Hosting**, garantissant ainsi une communication sécurisée entre le client et le serveur [oai_citation:2,spécification technique.pdf](file-service://file-1nTbGSoo0YhiLIAr3h43LVuj). 


### **3. Veille technologique** 
Avant de finaliser nos choix technologiques, nous avons mené une **veille technologique** approfondie. Pour cela, nous avons utilisé un outil comme **Wakelet** pour organiser et centraliser les informations. Afin
