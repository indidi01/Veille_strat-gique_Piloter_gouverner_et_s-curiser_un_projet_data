# Rapport de Veille — Pilotage, Stratégie, Gouvernance et Relation Client

## C1 — Pilotage de la veille et de l'innovation

> [!NOTE] 
> ### Contextualisation
>Pour TradeCorp une petite entreprise sans automatisation, la veille est un enjeu critique car l'information stratégique (concurrentielle, réglementaire, technologique) circule encore de manière informelle, par email, conversation ou mémoire individuelle. Sans processus structuré, l'entreprise risque de manquer des évolutions réglementaires (RGPD, AI Act) ou des opportunités technologiques qui pourraient transformer son positionnement. Mettre en place une veille organisée, même légère, est donc la première brique de toute stratégie data.

#### Agrégateurs de flux

| Outil | Description | Avantage | Inconvégnient |
| --- | --- | --- | --- |
| **Feedly** | Agrégateur RSS avec assistant IA (Leo) qui filtre et priorise les articles. | Interface soignée, IA de filtrage performante, intégrations Slack/Teams/Zapier, version gratuite (100 flux). | Version gratuite limitée, fonctionnalités IA réservées aux offres payantes ($6/mois). |
| **Inoreader** | Agrégateur RSS avancé avec règles d’automatisation et surveillance de sources non-RSS. | Version gratuite généreuse (150 flux), archive permanente, règles d’automatisation, surveillance de pages sans RSS. | Interface plus dense, courbe d’apprentissage plus raide. |
| **Google Alerts** | Service gratuit d’alertes par e-mail sur des mots-clés. | Gratuit, simplicité extrême, couverture de l’index Google. | Pas d’analyse de sentiment, sources limitées au web indexé, délais importants. |

#### Veille automatissé /IA

| Outil | Description | Avantages | Inconvénients |
|---|---|---|---|
| **Mention** | Outil de media monitoring qui suit en temps réel les mentions d’une marque ou de mots-clés sur le web, les réseaux sociaux, les blogs et les forums. | Couverture multicanale large, alertes en temps réel, interface simple, collaboration en équipe, rapports exportables. | Tarif élevé pour les petites structures, couverture limitée aux sources académiques ou techniques, peut générer beaucoup de bruit si les mots-clés sont mal paramétrés. |
| **Talkwalker** | Plateforme de social listening et d’analyse avancée qui mesure le sentiment, détecte les tendances et benchmarke les concurrents. | Analyse de sentiment fine, détection de tendances, benchmark concurrentiel, rapports très détaillés, couverture internationale. | Coût très élevé, orienté grands comptes et équipes marketing, courbe d’apprentissage importante, surdimensionné pour une équipe data réduite. |
| **Google Alerts** | Service gratuit qui envoie par e-mail des alertes lorsqu’un mot-clé apparaît dans les résultats Google. | Gratuit, extrêmement simple à configurer, aucune maintenance, fonctionne sans compte payant. | Pas d’analyse de sentiment, sources limitées au web indexé par Google, délais de notification, aucune gestion collaborative, pas d’archivage structuré. |

#### Curation et partage

| Outil | Description | Avantages | Inconvénients |
|---|---|---|---|
| **Pocket** | Application de sauvegarde d’articles pour lecture ultérieure, avec tags et recommandations. | Très simple d’utilisation, multiplateforme (web, mobile), intégrations nombreuses, mode hors-ligne. | Peu collaboratif, pas de base de connaissances structurée, pas d’agrégation RSS native, inadapté à une veille d’équipe. |
| **Diigo** | Outil de bookmarking social qui permet d’annoter, surligner et organiser des pages web en groupes collaboratifs. | Annotation collaborative, surlignage, recherche plein texte, archivage des pages, groupes de partage. | Interface datée, communauté moins active, fonctionnalités avancées payantes, peut paraître complexe pour un usage léger. |
| **Notion** | Outil tout-en-un de gestion de connaissances qui centralise articles, notes, tags et vues filtrées dans une base de données collaborative. | Très flexible, collaboratif en temps réel, centralise veille et documentation, gratuit pour petites équipes, vues personnalisables (tableau, kanban, calendrier). | Nécessite une discipline de structuration, pas d’agrégation RSS native (dépend d’intégrations type Zapier), peut devenir désordonné sans règles claires. |

### Tableau comparatif
### Recommandation
> [!TIP] 
>**Inoreader (version gratuite puis version pro à 7,50 $/mois)**
>
>Une équipe réduite ne peut pas se permettre de surveiller manuellement des dizaines de sources. Or, Inoreader offre dès sa version gratuite 150 flux (contre 100 pour Feedly) et intègre des règles d'automatisation qui permettent de taguer, filtrer et router automatiquement les articles vers des dossiers ou des canaux Slack. Cette automatisation est critique pour une équipe de 3 à 5 data engineers qui n'ont pas de temps dédié à la veille. De plus, l'archive permanente d'Inoreader garantit qu'aucun article n'est perdu au fil du temps, répondant directement à l'exigence de « conservation » de l'information. Enfin, la capacité à surveiller des sources non-RSS (comme les pages de release notes de frameworks qui ne publient pas de flux) est un atout majeur pour une veille technologique sur des outils comme Apache Spark ou Kafka.
>
>Feedly serait préférable pour une équipe plus large bénéficiant d'un budget confortable et privilégiant la simplicité. Google Alerts, bien que gratuit, est insuffisant car il ne couvre pas les sources sociales et ne permet aucune automatisation.

>[!TIP]
>**Mention**
>
>la nécessité de détecter rapidement les signaux faibles sur les réseaux sociaux et les forums, où les utilisateurs expriment leurs frustrations ou leurs attentes. Une petite équipe data n’a pas les ressources pour surveiller manuellement ces canaux. Mention offre une couverture multicanale (web, social, blogs, forums), des alertes en temps réel et une collaboration en équipe, ce qui permet de réagir vite à une vague de mécontentement ou à une tendance émergente. Talkwalker est trop coûteux et surdimensionné pour une équipe de 3 à 5 personnes. Google Alerts, bien que gratuit, ne couvre pas les réseaux sociaux et n’offre ni analyse de sentiment ni gestion collaborative. Mention est donc le meilleur compromis entre couverture, réactivité et budget.

>[!TIP]
>**Notion**
>
>la centralisation de la veille dans un espace collaboratif unique, accessible à l’équipe data mais aussi aux équipes produit et DSI. Notion permet de créer une base de veille avec tags, vues filtrées, notes et statuts, tout en centralisant la documentation existante. Pocket est trop individuel et inadapté à un partage d’équipe. Diigo, bien que collaboratif, souffre d’une interface datée et d’une communauté moins active. Notion est gratuit pour les petites équipes, flexible et s’intègre naturellement aux workflows déjà en place. Il répond à l’exigence de diffusion et de conservation de l’information sans ajouter de complexité technique.

### Limite 
>[!CAUTION]
>Inoreader ne résout pas le problème de la qualification de l'information, il collecte et filtre, mais ne dit pas si une mise à jour réglementaire est réellement applicable à TradeCorp ou si une nouvelle version de framework vaut la peine d'être adoptée. Cette analyse d'impact reste manuelle et dépend de la compétence des data engineers.

>[!CAUTION]
>
>Mention ne résout pas la veille réglementaire spécialisée (RGPD, AI Act), il excelle sur les signaux sociaux et médiatiques, mais ne remplace pas un suivi structuré des textes officiels et des normes. De plus, son coût récurrent peut peser sur le budget d’une petite structure.

>[!CAUTION]
>
>Notion n’agrège pas nativement les flux RSS, il dépend d’intégrations externes (Zapier, Make) pour automatiser la collecte, ce qui ajoute une dépendance technique. De plus, sans discipline de structuration, la base de veille peut rapidement devenir désordonnée et perdre sa valeur d’usage.

## C2 — Manager l'innovation (technologique, organisationnelle, économique)

> [!NOTE]
> ### Contextualisation
> TradeCorp, petite entreprise sans automatisation, ne peut pas se permettre d’innover par effet de mode. L’équipe data de 3 à 5 personnes doit évaluer rapidement la plus-value d’une technologie, son coût et son impact RSE (ODD 9, réduction de l’empreinte carbone). Un processus d’innovation léger, du prototype au MVP, est nécessaire pour éviter les investissements inutiles.

#### Prototypage / conception

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **Figma** | Outil de design collaboratif pour maquettes et prototypes interactifs. | Gratuit pour petites équipes, collaboration temps réel, prototypage rapide, nombreuses intégrations. | Nécessite une compétence design, limité aux interfaces, pas de prototypage hardware. |
| **Miro** | Tableau blanc collaboratif pour design thinking et cartes mentales. | Très visuel, idéal pour ateliers, templates variés, version gratuite. | Peut devenir désordonné, pas de prototypage fonctionnel, dépendance à la connexion. |
| **Balsamiq** | Outil de wireframing rapide à faible fidélité. | Prise en main immédiate, focus sur la structure, bibliothèque de composants. | Esthétique limitée, moins collaboratif que Figma, payant au-delà d’essai. |

#### Gestion de l’innovation

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **Lean Canvas** | Adaptation du Business Model Canvas pour startups, centrée problème/solution. | Rapide à remplir, focalise sur le risque, adapté aux petites équipes, gratuit. | Moins complet que BMC, peut simplifier à l’excès, nécessite itérations. |
| **Matrice d’Ansoff** | Matrice stratégique croisant produits et marchés. | Vision claire des options de croissance, simple à comprendre. | Statique, peu adaptée à l’innovation technologique rapide, ne dit pas comment exécuter. |
| **Business Model Canvas** | Modèle visuel en 9 blocs pour décrire un business model. | Holistique, standard, collaboratif. | Lourd pour une petite équipe, peut décourager l’itération rapide. |

#### Mesure d’impact environnemental

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **GreenIT-Analysis** | Extension navigateur pour analyser l’empreinte carbone d’une page web. | Gratuit, facile, indicateurs concrets, conforme RGESN. | Limité aux pages web, pas à l’infrastructure data complète. |
| **EcoIndex** | Outil de calcul de l’empreinte environnementale d’une page web. | Gratuit, score simple, bon pour sensibiliser. | Périmètre restreint, ne couvre pas le cloud/on-premise. |
| **Website Carbon Calculator** | Estime les émissions CO2 d’un site web. | Simple, rapide, pédagogique. | Approximatif, peu actionnable pour une infra data. |

### Tableau comparatif

### Recommandation

> [!TIP]
> **Figma**
> Pour une équipe réduite, Figma permet de prototyper rapidement des interfaces sans développement, ce qui réduit le risque de construire une fonctionnalité inutile. Sa version gratuite suffit pour 3-5 personnes, et son intégration avec Notion/Jira fluidifie le passage du prototype au backlog.

> [!TIP]
> **Lean Canvas**
> TradeCorp doit valider ses innovations avec un minimum de ressources. Lean Canvas force à formuler problème, solution, métriques et avantage déloyal en une page. Ansoff est trop macro et BMC trop lourd pour une itération hebdomadaire.

> [!TIP]
> **GreenIT-Analysis**
> Pour intégrer l’ODD 9, GreenIT-Analysis donne un indicateur rapide et gratuit de l’empreinte d’une interface. Il sensibilise l’équipe sans ajouter de complexité. Website Carbon est trop approximatif, EcoIndex trop limité.

### Limite

> [!CAUTION]
> Figma ne remplace pas les tests utilisateurs réels, un prototype peut sembler convaincant sans valider le besoin métier.

> [!CAUTION]
> Lean Canvas ne garantit pas la faisabilité technique ni la scalabilité, il faut ensuite un prototypage et des tests de charge.

> [!CAUTION]
> GreenIT-Analysis ne mesure pas l’empreinte de l’infrastructure data (cloud, stockage, calcul) , il faut compléter par une analyse cloud spécifique.

---

## C3 — Identifier les attentes et besoins utilisateurs/DSI

> [!NOTE]
> ### Contextualisation
> TradeCorp reçoit des demandes clients floues, souvent par email ou conversation informelle. Sans formalisation, l’équipe data risque de développer la mauvaise solution. De plus, l’accessibilité numérique (RGAA/WCAG) devient une obligation légale et un critère de qualité pour les interfaces destinées aux clients.

#### Recueil de besoins / specs

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **Notion** | Base de connaissances collaborative pour recueillir besoins, user stories et specs. | Flexible, gratuit petites équipes, centralise docs et veille, vues filtrées. | Nécessite discipline, pas de gestion de sprint native. |
| **Confluence** | Wiki d’entreprise pour documenter specs et processus. | Structuré, versionné, intégration Jira, bon pour équipes. | Payant, peut devenir rigide, administration plus lourde. |
| **Jira** | Outil de gestion de projet agile pour epics/user stories. | Suivi précis, workflow personnalisable, intégration dev. | Complexe pour non-techniques, coût par utilisateur. |

#### Modélisation de processus métier

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **Draw.io** | Outil de diagramme gratuit pour BPMN, UML, flux. | Gratuit, simple, intégration Google Drive/Notion, export multiple. | Pas de collaboration temps réel avancée, pas de validation de processus. |
| **Lucidchart** | Plateforme collaborative de diagrammes BPMN. | Templates BPMN, collaboration temps réel, intégrations. | Version gratuite limitée, payant pour équipes. |
| **BPMN (méthode)** | Notation standard pour modéliser processus métier. | Standard, lisible par métier et IT, précise. | Nécessite formation, peut être trop formel pour petits processus. |

#### Test d’accessibilité

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **WAVE** | Extension d’évaluation d’accessibilité web. | Gratuit, visuel, détecte erreurs WCAG, facile. | Limité à une page, ne teste pas les parcours complets. |
| **Lighthouse** | Audit automatisé Google pour performance et accessibilité. | Intégré Chrome, gratuit, scores clairs, CI possible. | Automatique seulement, ne remplace pas test manuel. |
| **Axe DevTools** | Extension de test d’accessibilité pour développeurs. | Précis, peu de faux positifs, intégration CI. | Version gratuite limitée, nécessite compétence technique. |

### Tableau comparatif

### Recommandation

> [!TIP]
> **Notion**
> Pour une équipe de 3-5 personnes, Notion centralise besoins, user stories et documentation sans coût supplémentaire. Il est plus souple que Confluence et plus accessible que Jira pour les métiers. Jira reste utile pour le suivi sprint, mais Notion suffit pour le recueil.

> [!TIP]
> **Draw.io**
> Draw.io est gratuit, simple et suffisant pour modéliser les processus métier de TradeCorp. Lucidchart est plus collaboratif mais payant. BPMN seul est une notation, pas un outil. Draw.io permet de passer rapidement du schéma au partage.

> [!TIP]
> **WAVE**
> WAVE est gratuit et visuel, idéal pour sensibiliser l’équipe à l’accessibilité sans compétence experte. Lighthouse est complémentaire pour la CI, mais WAVE reste le meilleur point d’entrée pour une petite structure.

### Limite

> [!CAUTION]
> Notion ne remplace pas un cahier des charges formel signé, il peut manquer de traçabilité contractuelle.

> [!CAUTION]
> Draw.io ne valide pas les processus avec les métiers, la modélisation doit être accompagnée d’ateliers.

> [!CAUTION]
> WAVE ne couvre pas tous les handicaps (auditif, cognitif) et ne remplace pas un audit RGAA complet.

---

## C5 — Diagnostiquer la problématique (environnement interne/externe)

> [!NOTE]
> ### Contextualisation
> TradeCorp doit diagnostiquer son SI avant toute migration cloud ou scalabilité. L’absence d’automatisation rend l’architecture existante difficile à évaluer. Un diagnostic interne/externe et des tests de charge permettent d’identifier les faiblesses sans mettre en production une infrastructure instable.

#### Diagnostic stratégique

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **SWOT** | Analyse forces/faiblesses/opportunités/menaces. | Simple, rapide, vision interne/externe. | Statique, subjectif, ne priorise pas. |
| **PESTEL** | Analyse macro-environnementale (politique, économique, social, technologique, écologique, légal). | Cadre large, utile pour veille réglementaire. | Long, peut être trop général, peu actionnable seul. |
| **5 forces de Porter** | Analyse concurrentielle du secteur. | Structure l’analyse marché, aide à positionner TradeCorp. | Orienté industrie, moins adapté aux petites structures agiles. |

#### Audit technique d’architecture

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **Well-Architected Framework** | Cadre AWS/Azure pour évaluer architecture cloud (sécurité, coût, fiabilité, performance, excellence opérationnelle, durabilité). | Structuré, bonnes pratiques, priorisation des risques. | Orienté cloud, nécessite expertise, peut être lourd. |
| **C4 Model** | Méthode de diagrammes d’architecture (contexte, conteneurs, composants, code). | Clair, adaptable, facilite communication. | Pas un audit, ne détecte pas les faiblesses seul. |
| **Benchmark technique** | Comparaison avec solutions similaires. | Identifie écarts, inspire bonnes pratiques. | Difficile à objectiver, dépend des données disponibles. |

#### Tests de charge / scalabilité

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **Apache JMeter** | Outil de test de charge open source. | Mature, extensible, supporte nombreux protocoles. | Interface datée, courbe d’apprentissage. |
| **k6** | Outil de test de charge scriptable en JavaScript. | Moderne, léger, CI-friendly, résultats clairs. | Nécessite compétences JS, moins de protocoles. |
| **Locust** | Test de charge en Python, distribué. | Code Python, scalable, interface web. | Nécessite développement, moins plug-and-play. |

### Tableau comparatif

### Recommandation

> [!TIP]
> **SWOT**
> Pour TradeCorp, le SWOT est le point de départ le plus rapide pour croiser interne/externe sans mobiliser un consultant. PESTEL et Porter sont trop lourds pour une première analyse, ils pourront compléter ensuite.

> [!TIP]
> **Well-Architected Framework**
> Ce cadre aide à diagnostiquer les faiblesses d’un SI cloud selon des critères reconnus (sécurité, coût, fiabilité). C4 Model est utile pour documenter, mais ne remplace pas un audit. Le framework donne une feuille de route priorisée.

> [!TIP]
> **k6**
> k6 est léger, scriptable et s’intègre en CI, ce qui convient à une petite équipe data. JMeter est plus lourd. Locust demande plus de code. k6 permet de tester la scalabilité avant production sans infrastructure complexe.

### Limite

> [!CAUTION]
> SWOT reste subjectif et ne mesure pas la faisabilité technique, il doit être confronté à l’audit.

> [!CAUTION]
> Well-Architected Framework est orienté cloud et ne couvre pas les spécificités data/IA (MLOps, lineage).

> [!CAUTION]
> k6 ne teste pas la sécurité ni la résilience en cas de panne réelle, il faut compléter par des tests de chaos.

---

## C6 — Définir une stratégie data/IA et un plan d’action

> [!NOTE]
> ### Contextualisation
> TradeCorp doit aligner sa stratégie data sur ses objectifs business et sécuriser ses données. Sans priorisation par le risque, l’équipe risque de tout traiter en même temps. La triade CIA (confidentialité, intégrité, disponibilité) et une roadmap IA réaliste sont nécessaires pour éviter les projets non maîtrisés.

#### Cadres de sécurité des données

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **ISO 27001** | Norme internationale de management de la sécurité de l’information. | Reconnue, structurante, auditables. | Lourde, coûteuse, nécessite certification. |
| **ISO 27018** | Extension pour la protection des données personnelles dans le cloud. | Spécifique cloud, rassurante pour clients. | Peu connue, périmètre restreint. |
| **NIST Cybersecurity Framework** | Cadre de cybersécurité américain (identifier, protéger, détecter, répondre, récupérer). | Flexible, gratuit, adaptable PME. | Non certifiant, nécessite traduction opérationnelle. |

#### Gestion de roadmap stratégique

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **Notion** | Base collaborative pour roadmap, priorités, statuts. | Gratuit, flexible, centralise docs. | Pas de dépendances avancées, discipline requise. |
| **ProductPlan** | Outil dédié à la roadmap produit. | Visualisation claire, collaboration, intégrations. | Payant, surdimensionné pour petite équipe. |
| **Aha!** | Plateforme de roadmap et gestion d’idées. | Complet, alignement stratégique, reporting. | Coût élevé, complexe. |

#### Cadres de mise en production IA (MLOps)

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **MLflow** | Plateforme open source pour cycle de vie ML (tracking, modèles, déploiement). | Gratuit, standard, extensible, communauté. | Nécessite infra, pas de gouvernance clé en main. |
| **Kubeflow** | Plateforme MLOps sur Kubernetes. | Scalable, pipeline complet, cloud-native. | Complexe à opérer, surdimensionné pour petite équipe. |
| **Azure ML** | Service managé de MLOps. | Intégré Azure, managé, sécurité. | Coût, dépendance fournisseur. |

### Tableau comparatif

### Recommandation

> [!TIP]
> **NIST Cybersecurity Framework**
> Pour TradeCorp, le NIST CSF est gratuit, flexible et proportionné à une PME. ISO 27001 est trop lourd à court terme, ISO 27018 est trop spécifique. Le NIST permet de prioriser les actions selon les risques.

> [!TIP]
> **Notion**
> Notion suffit pour une roadmap data/IA légère, avec priorités, responsables et échéances. ProductPlan et Aha! sont payants et surdimensionnés pour 3-5 personnes.

> [!TIP]
> **MLflow**
> MLflow est open source, standard et permet de tracer les expériences et modèles sans coût de licence. Kubeflow est trop complexe. Azure ML crée une dépendance. MLflow reste adapté à une équipe réduite.

### Limite

> [!CAUTION]
> Le NIST CSF ne fournit pas de mesures techniques prêtes à l’emploi, il faut les traduire en actions concrètes.

> [!CAUTION]
> Notion ne gère pas les dépendances complexes ni les ressources, il peut devenir un simple tableau si la gouvernance n’est pas définie.

> [!CAUTION]
> MLflow ne couvre pas la gouvernance des données ni la conformité RGPD, il faut le coupler à un catalogue et à des politiques.

---

## C9 — Développer la relation client et sa fidélisation

> [!NOTE]
> ### Contextualisation
> TradeCorp, en B2B, dépend d’un nombre limité de clients. La fidélisation est donc vitale. Sans CRM ni mesure de satisfaction, l’équipe risque de perdre des comptes sans signaux d’alerte. Le NPS et un suivi structuré des comptes permettent de prioriser les actions commerciales.

#### CRM

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **HubSpot** | CRM orienté PME avec marketing, ventes, service. | Gratuit, simple, écosystème complet, bon pour B2B. | Fonctions avancées payantes, peut devenir cher. |
| **Salesforce** | CRM grand compte très personnalisable. | Puissant, écosystème, reporting avancé. | Coûteux, complexe, nécessite admin. |
| **Zoho CRM** | CRM abordable pour PME. | Prix compétitif, fonctionnalités complètes, intégrations. | Interface moins intuitive, support variable. |
| **Pipedrive** | CRM centré pipeline de vente. | Visuel, simple, efficace pour petites équipes. | Moins complet en marketing/service. |

#### Mesure de satisfaction

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **Typeform** | Création d’enquêtes NPS et formulaires. | Interface agréable, logique conditionnelle, intégrations. | Version gratuite limitée, coût par réponse. |
| **SurveyMonkey** | Plateforme d’enquêtes. | Mature, templates NPS, analyse. | Payant pour fonctions avancées, moins design. |
| **Google Forms** | Formulaire gratuit. | Gratuit, simple, intégré Google. | Peu de logique, analyse limitée, design basique. |

#### Gestion de compte client

| Outil | Description | Avantages | Inconvénients |
| --- | --- | --- | --- |
| **Notion** | Base collaborative pour suivi de comptes, contacts, actions. | Flexible, gratuit, centralise notes. | Pas de CRM natif, automatisation limitée. |
| **Monday.com** | Plateforme de gestion de travail et suivi client. | Visuel, automations, collaboration. | Payant, peut être surdimensionné. |
| **Excel/Google Sheets** | Tableur pour suivi simple. | Gratuit, maîtrisé, flexible. | Pas de collaboration avancée, erreurs, pas d’alertes. |

### Tableau comparatif

### Recommandation

> [!TIP]
> **HubSpot**
> HubSpot offre un CRM gratuit et complet pour une PME B2B comme TradeCorp. Il est plus simple que Salesforce et plus complet que Pipedrive. La version gratuite permet de démarrer sans budget, puis d’évoluer.

> [!TIP]
> **Typeform**
> Typeform est idéal pour envoyer des NPS courts et engageants. SurveyMonkey est plus lourd. Google Forms trop limité pour analyser les tendances. Typeform s’intègre au CRM pour automatiser les relances.

> [!TIP]
> **Notion**
> Pour une petite équipe, Notion suffit pour suivre les comptes, les échanges et les prochaines actions. Monday.com est payant et plus orienté gestion de projet. Notion centralise déjà la veille et les specs, évitant un nouvel outil.

### Limite

> [!CAUTION]
> HubSpot gratuit reste limité en automatisation et reporting, il ne remplace pas un CRM enterprise pour des besoins complexes.

> [!CAUTION]
> Le NPS est un indicateur déclaratif, il ne mesure pas le chiffre d’affaires réel ni la rétention.

> [!CAUTION]
> Notion n’est pas un CRM, sans processus de relance, il peut devenir un simple journal sans impact commercial.

## Synthèse finale — Priorisation pour TradeCorp

Parmi tous les thèmes traités, voici les 3 thèmes prioritaires à mettre en place en premier chez  TradeCorp, justifiés par leur urgence relative :

    C1 — Pilotage de la veille et de l'innovation
    Pourquoi en premier ? Sans veille structurée, TradeCorp ne peut ni anticiper les évolutions réglementaires (RGPD, AI Act) ni détecter les innovations technologiques qui pourraient menacer ou renforcer son positionnement. C'est la brique fondatrice de toute stratégie data, elle alimente les autres décisions. Inoreader (version gratuite) et Notion permettent de démarrer immédiatement, sans budget.

    C6 — Définir une stratégie data/IA et un plan d'action
    Pourquoi en deuxième ? Une fois la veille en place, TradeCorp doit clarifier sa stratégie de sécurisation des données et prioriser les actions par le risque. Le NIST CSF (gratuit) et MLflow (open source) permettent de structurer sans coût excessif. Sans cette étape, les projets data/IA risquent de se développer sans cadre, avec des risques de conformité et de sécurité.

    C9 — Développer la relation client et sa fidélisation
    Pourquoi en troisième ? TradeCorp dépend de ses clients B2B : la fidélisation est un enjeu de survie. HubSpot (gratuit) et Typeform permettent de mesurer le NPS et d'identifier les clients à risque, sans investissement lourd. Ce thème est prioritaire car il a un impact direct sur le chiffre d'affaires, mais il vient après la veille et la stratégie data car il s'appuie sur des données fiables et une organisation structurée.

Pourquoi pas les autres ?
Les thèmes C2 (innovation), C3 (besoins utilisateurs), C5 (diagnostic) et les autres sont importants mais moins urgents, ils supposent que la veille, la stratégie data et la relation client soient déjà en place. La gouvernance des données et la gestion des risques sont également critiques, mais elles peuvent être traitées dans un second temps, une fois les fondations posées. TradeCorp doit éviter de se disperser, mieux vaut trois thèmes traités en profondeur que dix survolés.

---

## Glossaire

| Terme | Définition |
|---|---|
| **Veille technologique** | Observer, collecter, analyser et diffuser des informations sur les nouveautés techniques et scientifiques pour anticiper les évolutions d’un secteur. |
| **Veille concurrentielle** | Collecter et analyser des informations sur les actions, les produits et les stratégies des concurrents pour anticiper les mouvements du marché. |
| **Curation de contenu** | Pratique qui consiste à rechercher, trier, sélectionner et partager les informations ou médias les plus pertinents du web sur un sujet précis. |
| **Agrégateur RSS** | Outil qui rassemble sur une seule interface les nouveautés et articles de plusieurs sites web ou blogs. |
| **Alerte Google** | Service gratuit de Google qui envoie un e-mail dès qu’une nouvelle page web correspond à des mots-clés choisis. |
| **Outil de veille automatisée** | Logiciel qui surveille Internet et collecte des informations utiles en continu, sans recherche manuelle. |
| **Design thinking** | Démarche de conception centrée sur l’utilisateur, itérative, qui alterne empathie, définition, idéation, prototypage et test. |
| **Prototypage rapide** | Création rapide de maquettes ou de versions simplifiées d’un produit pour tester des hypothèses et recueillir des retours. |
| **Lean startup** | Méthode de développement de produit qui privilégie l’expérimentation, le MVP et l’apprentissage validé pour réduire les risques. |
| **MVP (Minimum Viable Product)** | Version minimale d’un produit contenant juste assez de fonctionnalités pour être testée auprès des premiers utilisateurs. |
| **Matrice d’innovation** | Outil de classification des innovations selon leur degré de nouveauté (incrémentale, adjacente, radicale) et leur impact. |
| **Green IT** | Ensemble de pratiques visant à réduire l’empreinte environnementale des technologies de l’information (matériel, logiciel, usages). |
| **Empreinte carbone du numérique** | Quantité de gaz à effet de serre émise par les équipements, réseaux, centres de données et services numériques. |
| **ODD 9** | Objectif de Développement Durable n°9 des Nations Unies : bâtir une infrastructure résiliente, promouvoir une industrialisation durable et encourager l’innovation. |
| **Recueil de besoins** | Processus de collecte et de formalisation des attentes des utilisateurs ou parties prenantes pour définir un projet. |
| **Cahier des charges fonctionnel** | Document qui décrit les besoins fonctionnels, les contraintes et les critères d’acceptation d’un projet. |
| **User story** | Description courte d’une fonctionnalité du point de vue de l’utilisateur, souvent au format « En tant que… je veux… afin de… ». |
| **Persona** | Profil fictif représentant un groupe d’utilisateurs cibles, utilisé pour guider la conception. |
| **Accessibilité numérique** | Ensemble de règles et bonnes pratiques permettant à tous, y compris les personnes handicapées, d’accéder aux services numériques. |
| **RGAA** | Référentiel Général d’Amélioration de l’Accessibilité : cadre français pour rendre les sites et applications accessibles. |
| **WCAG** | Web Content Accessibility Guidelines : normes internationales d’accessibilité des contenus web. |
| **Analyse SWOT** | Analyse des forces (Strengths), faiblesses (Weaknesses), opportunités (Opportunities) et menaces (Threats) d’une organisation. |
| **Analyse PESTEL** | Analyse des facteurs externes : Politiques, Économiques, Socioculturels, Technologiques, Écologiques et Légaux. |
| **Audit d’architecture SI** | Évaluation de l’architecture du système d’information pour identifier les forces, faiblesses et axes d’amélioration. |
| **Scalabilité horizontale** | Capacité à augmenter la puissance en ajoutant des machines ou nœuds supplémentaires. |
| **Scalabilité verticale** | Capacité à augmenter la puissance en ajoutant des ressources (CPU, RAM) à une machine existante. |
| **Benchmark technique** | Comparaison de solutions ou architectures sur des critères définis (performance, coût, complexité) pour choisir objectivement. |
| **Data strategy** | Stratégie d’entreprise définissant comment les données sont collectées, stockées, gouvernées, analysées et valorisées. |
| **Architecture data-driven** | Organisation dont les décisions et processus s’appuient systématiquement sur l’analyse de données. |
| **Triade CIA** | Confidentialité, Intégrité, Disponibilité : les trois piliers de la sécurité de l’information. |
| **Matrice de risques** | Outil de priorisation des risques selon leur probabilité et leur impact. |
| **Roadmap IA** | Feuille de route décrivant les étapes, priorités et livrables pour intégrer l’IA dans une organisation. |
| **MLOps** | Ensemble de pratiques pour industrialiser le cycle de vie des modèles de machine learning (développement, déploiement, monitoring). |
| **CRM** | Customer Relationship Management : outil de gestion de la relation client (contacts, interactions, pipeline commercial). |
| **Fidélisation client B2B** | Ensemble d’actions visant à maintenir et développer la relation avec des clients professionnels sur le long terme. |
| **NPS** | Net Promoter Score : indicateur de satisfaction client basé sur la probabilité de recommandation. |
| **Techniques de négociation commerciale** | Méthodes pour parvenir à un accord gagnant-gagnant avec un client ou partenaire (BATNA, ancrage, concessions). |
| **Account management** | Gestion d’un portefeuille de clients stratégiques, avec suivi personnalisé et développement de la relation. |
| **KPI projet data** | Indicateurs clés de performance spécifiques aux projets data (taux d’erreur, latence, coût, vélocité). |
| **ROI IA** | Retour sur investissement des projets d’intelligence artificielle : bénéfices mesurables par rapport aux coûts engagés. |
| **OKR** | Objectives and Key Results : méthode de définition d’objectifs ambitieux et de résultats mesurables. |
| **Post-mortem de projet** | Analyse rétrospective d’un projet terminé pour identifier les réussites, échecs et axes d’amélioration. |
| **Vélocité d’équipe** | Quantité de travail (souvent en points de story) qu’une équipe agile réalise lors d’un sprint. |
| **Management agile** | Approche de gestion d’équipe favorisant l’itération, l’autonomie, la collaboration et l’adaptation au changement. |
| **Scrum Master** | Facilitateur de l’équipe Scrum, garant du respect du cadre agile et de la levée des obstacles. |
| **Rétrospective d’équipe** | Réunion périodique où l’équipe analyse son fonctionnement pour améliorer ses pratiques. |
| **1-to-1 manager** | Entretien individuel régulier entre un manager et un collaborateur pour faire le point et développer les compétences. |
| **Matrice RACI** | Outil de clarification des rôles : Responsible, Accountable, Consulted, Informed pour chaque tâche. |
| **Gouvernance des données** | Ensemble de règles, processus et responsabilités pour garantir la qualité, la sécurité et la valorisation des données. |
| **Data catalog** | Inventaire structuré des données de l’entreprise (sources, descriptions, propriétaires, sensibilité). |
| **Data lineage** | Traçabilité du parcours d’une donnée, depuis sa source jusqu’à son utilisation finale. |
| **Plan de Gouvernance des Données (PGD)** | Document stratégique définissant les principes, rôles et processus de gouvernance des données. |
| **DAMA-DMBOK** | Référentiel de bonnes pratiques en gouvernance des données, couvrant 11 domaines (qualité, sécurité, metadata, etc.). |
| **Analyse de risques EBIOS RM** | Méthode ANSSI d’analyse des risques cyber en 5 ateliers, adaptée aux PME et aux organismes publics. |
| **Matrice probabilité/impact** | Outil visuel de priorisation des risques selon leur probabilité d’occurrence et leur impact. |
| **Plan de reprise d’activité (PRA)** | Procédure de restauration des systèmes et données après un sinistre majeur, avec objectifs de délai et de perte de données. |
| **Plan de continuité d’activité (PCA)** | Dispositif permettant de maintenir les activités essentielles en cas de crise (solutions de secours, procédures). |
| **Gestion de crise data** | Ensemble des actions de coordination, communication et remédiation en cas d’incident majeur sur les données. |

---

## Sources consultées

- Feedly : [https://feedly.com](https://feedly.com)
- Inoreader : [https://www.inoreader.com](https://www.inoreader.com)
- Google Alerts : [https://www.google.com/alerts](https://www.google.com/alerts)
- Mention : [https://mention.com](https://mention.com)
- Talkwalker : [https://www.talkwalker.com](https://www.talkwalker.com)
- Pocket : [https://getpocket.com](https://getpocket.com)
- Diigo : [https://www.diigo.com](https://www.diigo.com)
- Notion : [https://www.notion.so](https://www.notion.so)
- Figma : [https://www.figma.com](https://www.figma.com)
- Miro : [https://miro.com](https://miro.com)
- Balsamiq : [https://balsamiq.com](https://balsamiq.com)
- EcoIndex : [https://www.ecoindex.fr](https://www.ecoindex.fr)
- Website Carbon Calculator : [https://www.websitecarbon.com](https://www.websitecarbon.com)
- GreenIT-Analysis : [https://www.greenit-analysis.com](https://www.greenit-analysis.com)
- Confluence : [https://www.atlassian.com/software/confluence](https://www.atlassian.com/software/confluence)
- Jira : [https://www.atlassian.com/software/jira](https://www.atlassian.com/software/jira)
- Lucidchart : [https://www.lucidchart.com](https://www.lucidchart.com)
- Draw.io : [https://www.drawio.com](https://www.drawio.com)
- WAVE : [https://wave.webaim.org](https://wave.webaim.org)
- Lighthouse : [https://developer.chrome.com/docs/lighthouse](https://developer.chrome.com/docs/lighthouse)
- Axe DevTools : [https://www.deque.com/axe/devtools](https://www.deque.com/axe/devtools)
- Well-Architected Framework : [https://aws.amazon.com/architecture/well-architected](https://aws.amazon.com/architecture/well-architected)
- C4 Model : [https://c4model.com](https://c4model.com)
- Apache JMeter : [https://jmeter.apache.org](https://jmeter.apache.org)
- k6 : [https://k6.io](https://k6.io)
- Locust : [https://locust.io](https://locust.io)
- ISO 27001 : [https://www.iso.org/isoiec-27001-information-security.html](https://www.iso.org/isoiec-27001-information-security.html)
- ISO 27018 : [https://www.iso.org/standard/76559.html](https://www.iso.org/standard/76559.html)
- NIST Cybersecurity Framework : [https://www.nist.gov/cyberframework](https://www.nist.gov/cyberframework)
- ProductPlan : [https://www.productplan.com](https://www.productplan.com)
- Aha! : [https://www.aha.io](https://www.aha.io)
- MLflow : [https://mlflow.org](https://mlflow.org)
- Kubeflow : [https://www.kubeflow.org](https://www.kubeflow.org)
- Azure ML : [https://azure.microsoft.com/en-us/products/machine-learning](https://azure.microsoft.com/en-us/products/machine-learning)
- Salesforce : [https://www.salesforce.com](https://www.salesforce.com)
- HubSpot : [https://www.hubspot.com](https://www.hubspot.com)
- Zoho CRM : [https://www.zoho.com/crm](https://www.zoho.com/crm)
- Pipedrive : [https://www.pipedrive.com](https://www.pipedrive.com)
- Typeform : [https://www.typeform.com](https://www.typeform.com)
- SurveyMonkey : [https://www.surveymonkey.com](https://www.surveymonkey.com)
- Monday.com : [https://monday.com](https://monday.com)
- Power BI : [https://powerbi.microsoft.com](https://powerbi.microsoft.com)
- Tableau : [https://www.tableau.com](https://www.tableau.com)
- Looker Studio : [https://lookerstudio.google.com](https://lookerstudio.google.com)
- Retrium : [https://www.retrium.com](https://www.retrium.com)
- Linear : [https://linear.app](https://linear.app)
- Trello : [https://trello.com](https://trello.com)
- Slack : [https://slack.com](https://slack.com)
- Microsoft Teams : [https://www.microsoft.com/en-us/microsoft-teams](https://www.microsoft.com/en-us/microsoft-teams)
- Microsoft Purview : [https://azure.microsoft.com/en-us/products/purview](https://azure.microsoft.com/en-us/products/purview)
- Collibra : [https://www.collibra.com](https://www.collibra.com)
- Atlan : [https://atlan.com](https://atlan.com)
- Apache Atlas : [https://atlas.apache.org](https://atlas.apache.org)
- OpenLineage : [https://openlineage.io](https://openlineage.io)
- DAMA-DMBOK : [https://www.dama.org](https://www.dama.org)
- EBIOS RM : [https://www.ssi.gouv.fr/guide/ebios-risk-manager](https://www.ssi.gouv.fr/guide/ebios-risk-manager)
- ISO 27005 : [https://www.iso.org/standard/80585.html](https://www.iso.org/standard/80585.html)
- Azure Backup : [https://azure.microsoft.com/en-us/products/backup](https://azure.microsoft.com/en-us/products/backup)
- RGAA : [https://www.numerique.gouv.fr/publications/rgaa-accessibilite](https://www.numerique.gouv.fr/publications/rgaa-accessibilite)
- WCAG : [https://www.w3.org/WAI/standards-guidelines/wcag](https://www.w3.org/WAI/standards-guidelines/wcag)
- ODD 9 : [https://www.un.org/sustainabledevelopment/fr/infrastructure](https://www.un.org/sustainabledevelopment/fr/infrastructure)