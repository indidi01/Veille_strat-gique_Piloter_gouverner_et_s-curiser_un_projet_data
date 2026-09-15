# Rapport de Veille — Pilotage, Stratégie, Gouvernance et Relation Client

## C1 — Pilotage de la veille et de l'innovation

> [!NOTE] 
> ### Contextualisation
>Pour une petite entreprise sans automatisation, la veille est un enjeu critique car l'information stratégique (concurrentielle, réglementaire, technologique) circule encore de manière informelle, par email, conversation ou mémoire individuelle. Sans processus structuré, l'entreprise risque de manquer des évolutions réglementaires (RGPD, AI Act) ou des opportunités technologiques qui pourraient transformer son positionnement. Mettre en place une veille organisée, même légère, est donc la première brique de toute stratégie data.

### Tableau comparatif

#### Agrégateurs de flux

| Outil | Description | Avantage | Inconvégnient |
| --- | --- | --- | --- |
| **Feedly** | Agrégateur RSS avec assistant IA (Leo) qui filtre et priorise les articles. | Interface soignée, IA de filtrage performante, intégrations Slack/Teams/Zapier, version gratuite (100 flux). | Version gratuite limitée, fonctionnalités IA réservées aux offres payantes ($6/mois). |
| **Inoreader** | Agrégateur RSS avancé avec règles d’automatisation et surveillance de sources non-RSS. | Version gratuite généreuse (150 flux), archive permanente, règles d’automatisation, surveillance de pages sans RSS. | Interface plus dense, courbe d’apprentissage plus raide. |
| **Google Alerts** | Service gratuit d’alertes par e-mail sur des mots-clés. | Gratuit, simplicité extrême, couverture de l’index Google. | Pas d’analyse de sentiment, sources limitées au web indexé, délais importants. |

> [!TIP] 
> ### Recommandation
>**Inoreader (version gratuite puis version pro à 7,50 $/mois)**
>
>Ce choix se justifie par un critère précis lié au contexte de StreamVault : la petite taille de l'équipe data. Une équipe réduite ne peut pas se permettre de surveiller manuellement des dizaines de sources. Or, Inoreader offre dès sa version gratuite 150 flux (contre 100 pour Feedly) et intègre des règles d'automatisation qui permettent de taguer, filtrer et router automatiquement les articles vers des dossiers ou des canaux Slack. Cette automatisation est critique pour une équipe de 3 à 5 data engineers qui n'ont pas de temps dédié à la veille. De plus, l'archive permanente d'Inoreader garantit qu'aucun article n'est perdu au fil du temps, répondant directement à l'exigence de « conservation » de l'information. Enfin, la capacité à surveiller des sources non-RSS (comme les pages de release notes de frameworks qui ne publient pas de flux) est un atout majeur pour une veille technologique sur des outils comme Apache Spark ou Kafka.
>
>Feedly serait préférable pour une équipe plus large bénéficiant d'un budget confortable et privilégiant la simplicité. Google Alerts, bien que gratuit, est insuffisant car il ne couvre pas les sources sociales et ne permet aucune automatisation.

>[!CAUTION]
>### Limite 
>Inoreader ne résout pas le problème de la qualification de l'information, il collecte et filtre, mais ne dit pas si une mise à jour réglementaire est réellement applicable à StreamVault ou si une nouvelle version de framework vaut la peine d'être adoptée. Cette analyse d'impact reste manuelle et dépend de la compétence des data engineers.

#### Veille automatissé /IA

| Outil | Description | Avantages | Inconvénients |
|---|---|---|---|
| **Mention** | Outil de media monitoring qui suit en temps réel les mentions d’une marque ou de mots-clés sur le web, les réseaux sociaux, les blogs et les forums. | Couverture multicanale large, alertes en temps réel, interface simple, collaboration en équipe, rapports exportables. | Tarif élevé pour les petites structures, couverture limitée aux sources académiques ou techniques, peut générer beaucoup de bruit si les mots-clés sont mal paramétrés. |
| **Talkwalker** | Plateforme de social listening et d’analyse avancée qui mesure le sentiment, détecte les tendances et benchmarke les concurrents. | Analyse de sentiment fine, détection de tendances, benchmark concurrentiel, rapports très détaillés, couverture internationale. | Coût très élevé, orienté grands comptes et équipes marketing, courbe d’apprentissage importante, surdimensionné pour une équipe data réduite. |
| **Google Alerts** | Service gratuit qui envoie par e-mail des alertes lorsqu’un mot-clé apparaît dans les résultats Google. | Gratuit, extrêmement simple à configurer, aucune maintenance, fonctionne sans compte payant. | Pas d’analyse de sentiment, sources limitées au web indexé par Google, délais de notification, aucune gestion collaborative, pas d’archivage structuré. |


### Curation et partage

| Outil | Description | Avantages | Inconvénients |
|---|---|---|---|
| **Pocket** | Application de sauvegarde d’articles pour lecture ultérieure, avec tags et recommandations. | Très simple d’utilisation, multiplateforme (web, mobile), intégrations nombreuses, mode hors-ligne. | Peu collaboratif, pas de base de connaissances structurée, pas d’agrégation RSS native, inadapté à une veille d’équipe. |
| **Diigo** | Outil de bookmarking social qui permet d’annoter, surligner et organiser des pages web en groupes collaboratifs. | Annotation collaborative, surlignage, recherche plein texte, archivage des pages, groupes de partage. | Interface datée, communauté moins active, fonctionnalités avancées payantes, peut paraître complexe pour un usage léger. |
| **Notion** | Outil tout-en-un de gestion de connaissances qui centralise articles, notes, tags et vues filtrées dans une base de données collaborative. | Très flexible, collaboratif en temps réel, centralise veille et documentation, gratuit pour petites équipes, vues personnalisables (tableau, kanban, calendrier). | Nécessite une discipline de structuration, pas d’agrégation RSS native (dépend d’intégrations type Zapier), peut devenir désordonné sans règles claires. |



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