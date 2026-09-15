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
>Mention ne résout pas la veille réglementaire spécialisée (RGPD, AI Act) : il excelle sur les signaux sociaux et médiatiques, mais ne remplace pas un suivi structuré des textes officiels et des normes. De plus, son coût récurrent peut peser sur le budget d’une petite structure.

>[!CAUTION]
>
>Notion n’agrège pas nativement les flux RSS : il dépend d’intégrations externes (Zapier, Make) pour automatiser la collecte, ce qui ajoute une dépendance technique. De plus, sans discipline de structuration, la base de veille peut rapidement devenir désordonnée et perdre sa valeur d’usage.

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
> Figma ne remplace pas les tests utilisateurs réels : un prototype peut sembler convaincant sans valider le besoin métier.

> [!CAUTION]
> Lean Canvas ne garantit pas la faisabilité technique ni la scalabilité : il faut ensuite un prototypage et des tests de charge.

> [!CAUTION]
> GreenIT-Analysis ne mesure pas l’empreinte de l’infrastructure data (cloud, stockage, calcul) ; il faut compléter par une analyse cloud spécifique.

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
> Draw.io est gratuit, simple et suffisant pour modéliser les processus métier de TradeCorp. Lucidchart est plus collaboratif mais payant ; BPMN seul est une notation, pas un outil. Draw.io permet de passer rapidement du schéma au partage.

> [!TIP]
> **WAVE**
> WAVE est gratuit et visuel, idéal pour sensibiliser l’équipe à l’accessibilité sans compétence experte. Lighthouse est complémentaire pour la CI, mais WAVE reste le meilleur point d’entrée pour une petite structure.

### Limite

> [!CAUTION]
> Notion ne remplace pas un cahier des charges formel signé : il peut manquer de traçabilité contractuelle.

> [!CAUTION]
> Draw.io ne valide pas les processus avec les métiers : la modélisation doit être accompagnée d’ateliers.

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
> Pour TradeCorp, le SWOT est le point de départ le plus rapide pour croiser interne/externe sans mobiliser un consultant. PESTEL et Porter sont trop lourds pour une première analyse ; ils pourront compléter ensuite.

> [!TIP]
> **Well-Architected Framework**
> Ce cadre aide à diagnostiquer les faiblesses d’un SI cloud selon des critères reconnus (sécurité, coût, fiabilité). C4 Model est utile pour documenter, mais ne remplace pas un audit. Le framework donne une feuille de route priorisée.

> [!TIP]
> **k6**
> k6 est léger, scriptable et s’intègre en CI, ce qui convient à une petite équipe data. JMeter est plus lourd ; Locust demande plus de code. k6 permet de tester la scalabilité avant production sans infrastructure complexe.

### Limite

> [!CAUTION]
> SWOT reste subjectif et ne mesure pas la faisabilité technique : il doit être confronté à l’audit.

> [!CAUTION]
> Well-Architected Framework est orienté cloud et ne couvre pas les spécificités data/IA (MLOps, lineage).

> [!CAUTION]
> k6 ne teste pas la sécurité ni la résilience en cas de panne réelle ; il faut compléter par des tests de chaos.

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
> Pour TradeCorp, le NIST CSF est gratuit, flexible et proportionné à une PME. ISO 27001 est trop lourd à court terme ; ISO 27018 est trop spécifique. Le NIST permet de prioriser les actions selon les risques.

> [!TIP]
> **Notion**
> Notion suffit pour une roadmap data/IA légère, avec priorités, responsables et échéances. ProductPlan et Aha! sont payants et surdimensionnés pour 3-5 personnes.

> [!TIP]
> **MLflow**
> MLflow est open source, standard et permet de tracer les expériences et modèles sans coût de licence. Kubeflow est trop complexe ; Azure ML crée une dépendance. MLflow reste adapté à une équipe réduite.

### Limite

> [!CAUTION]
> Le NIST CSF ne fournit pas de mesures techniques prêtes à l’emploi : il faut les traduire en actions concrètes.

> [!CAUTION]
> Notion ne gère pas les dépendances complexes ni les ressources : il peut devenir un simple tableau si la gouvernance n’est pas définie.

> [!CAUTION]
> MLflow ne couvre pas la gouvernance des données ni la conformité RGPD : il faut le coupler à un catalogue et à des politiques.

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
> Typeform est idéal pour envoyer des NPS courts et engageants. SurveyMonkey est plus lourd ; Google Forms trop limité pour analyser les tendances. Typeform s’intègre au CRM pour automatiser les relances.

> [!TIP]
> **Notion**
> Pour une petite équipe, Notion suffit pour suivre les comptes, les échanges et les prochaines actions. Monday.com est payant et plus orienté gestion de projet. Notion centralise déjà la veille et les specs, évitant un nouvel outil.

### Limite

> [!CAUTION]
> HubSpot gratuit reste limité en automatisation et reporting : il ne remplace pas un CRM enterprise pour des besoins complexes.

> [!CAUTION]
> Le NPS est un indicateur déclaratif : il ne mesure pas le chiffre d’affaires réel ni la rétention.

> [!CAUTION]
> Notion n’est pas un CRM : sans processus de relance, il peut devenir un simple journal sans impact commercial.

---

## Annexe — Vocabulaire essentiel

| Terme | Définition |
|---|---|
| **La veille technologique** | consiste à observer, collecter, analyser et diffuser des informations sur les nouveautés techniques et scientifiques pour anticiper les évolutions d'un secteur|
| **veille consiste à rechercher** | consiste à collecter et analyser des informations sur les actions, les produits et les stratégies des concurrents pour anticiper les mouvements du marché|
| **curation de contenu** |pratique qui consiste à rechercher, trier, sélectionner et partager les informations ou les médias les plus pertinents du web sur un sujet précis|
| **agrégateur RSS** | outil qui rassemble sur une seule et même interface les nouveautés et les articles de plusieurs sites web ou blogs|
| **alerte Google** | un service gratuit de Google qui vous envoie un e-mail dès qu'une nouvelle page web correspond à des mots-clés que vous avez choisis|
| **outil de veille automatisée** | logiciel qui surveille Internet et collecte des informations utiles pour vous en continu, sans que vous ayez besoin de chercher manuellement|
| **Data Catalog** | Inventaire des données et de leurs métadonnées. |
| **Data Lineage** | Traçabilité du parcours et des transformations d'une donnée. |
| **Data Governance** | Règles, rôles et processus permettant de maîtriser les données. |
| **Data Quality** | Mesure de la qualité et de la fiabilité des données. |
| **MLOps** | Industrialisation du cycle de vie des modèles ML. |
| **RACI** | Méthode de répartition des responsabilités. |
| **KPI** | Indicateur de performance. |
| **OKR** | Objectifs associés à des résultats clés mesurables. |
| **SLA** | Engagement de niveau de service. |
| **RPO** | Quantité maximale de données acceptable à perdre. |
| **RTO** | Durée maximale acceptable pour restaurer un service. |
| **RBAC** | Contrôle d'accès basé sur les rôles. |
| **RDF** | Modèle de représentation des connaissances par triplets. |
| **OWL** | Langage permettant de formaliser une ontologie. |
| **Ontologie** | Modèle formel des concepts et relations d'un domaine. |
| **SPARQL** | Langage de requête pour les données RDF. |
| **SWOT** | Forces, faiblesses, opportunités, menaces. |
| **PESTEL** | Analyse de l'environnement externe. |
| **PCA** | Plan de continuité d'activité. |
| **PRA** | Plan de reprise d'activité. |
| **CIA** | Confidentialité, intégrité, disponibilité. |
| **EBIOS RM** | Méthode d'analyse des risques numériques de l'ANSSI. |
| **MLOps** | Ensemble de pratiques pour industrialiser et surveiller les modèles ML. |

---

## Sources consultées

1. PageCrawl — Best RSS Feed Monitoring Tools 2026 : https://pagecrawl.io/blog/best-rss-feed-monitoring-tools
2. Inoreader — Alternative to Feedly : https://www.inoreader.com/ca/alternative-to-feedly
3. StartPageHQ — Feedly vs Inoreader : https://startpagehq.com/compare/feedly-vs-inoreader
4. Miro — Lean Canvas vs Business Model Canvas : https://miro.com/strategic-planning/lean-canvas-vs-business-model-canvas/
5. Linden Innovation — BMC vs Lean Canvas : https://lindeninnovation.com/business-model-canvas-vs-lean-canvas/
6. Projet Celsius — Empreinte carbone site web : https://projetcelsius.com/blog/empreinte-carbone-site-internet-guide/
7. Eesel — Notion vs Confluence 2026 : https://www.eesel.ai/blog/notion-vs-confluence
8. Fabric — Notion vs Confluence 2026 : https://fabric.so/comparison/notion-vs-confluence
9. Crosscheck — axe vs WAVE vs Pa11y : https://crosscheck.cloud/blogs/axe-vs-wave-vs-pa11y-accessibility-testing/
10. SWOTPal — SWOT vs PESTLE vs Porter 2026 : https://swotpal.com/academy/swot-vs-pestle-vs-porters-five-forces
11. QAInsights — JMeter vs k6 vs Locust 2026 : https://qainsights.com/jmeter-vs-k6-vs-locust-in-2026-which-load-testing-tool-should-you-pick/
12. QASkills — k6 vs JMeter 2026 : https://qaskills.sh/blog/k6-vs-jmeter-2026
13. GetRoz — ISO 27001 vs NIST 2026 : https://www.getroz.com/blog/iso-27001-vs-nist
14. Cyber Academy — EBIOS RM vs ISO 27005 : https://cyberacademy.net/resources/pillars/ebios-rm-vs-iso-27005
15. Salesflare — Salesforce vs HubSpot vs Zoho vs Pipedrive 2026 : https://blog.salesflare.com/compare-salesforce-zoho-hubspot-pipedrive
16. GetPricePulse — CRM Pricing Guide 2026 : https://www.getpricepulse.com/blog/crm-pricing-guide-2026.html
17. QuestionPro — Typeform vs SurveyMonkey 2026 : https://www.questionpro.com/blog/typeform-vs-surveymonkey/
18. Hayot Expertise — Power BI vs Tableau vs Looker Studio 2026 : https://hayot-expertise.fr/en/blog/power-bi-vs-tableau-vs-looker-studio-reporting-sme-2026
19. Tech Insider — Trello vs Jira 2026 : https://tech-insider.org/trello-vs-jira-2026/
20. ONES — Linear vs Jira vs Trello : https://ones.com/blog/linear-vs-jira-vs-trello-5-scenarios-to-choose-the-best-fit/
21. Basedash — Best Data Catalog Tools 2026 : https://www.basedash.com/blog/best-data-catalog-tools-compared-2026
22. Atlan — DAMA-DMBOK Framework : https://atlan.com/dama-dmbok-framework/
23. Promethium — Data Governance Tools Comparison : https://promethium.ai/guides/data-governance-tools-comparison-collibra-alation-atlan-purview/
24. Devforma — EBIOS RM ISO NIS2 DORA : https://devforma.com/ebios-rm-iso-nis2-dora/
25. European Commission — AI Act : https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai
26. Legiscope — CMP Comparison 2026 : https://www.legiscope.com/blog/consent-management-platforms-compared.html
27. SecurePrivacy — Best CMP 2026 : https://secureprivacy.ai/blog/best-cmp-2026
28. European Commission — AI Act Enforcement 2026 : https://commission.europa.eu/news-and-media/news/safer-and-more-transparent-ai-2026-08-02_en