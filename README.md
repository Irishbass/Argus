# ARGUS

ARGUS est une plateforme d'intelligence documentaire basée sur l'intelligence artificielle dont l'objectif est de transformer automatiquement le code source en documentation fonctionnelle, structurée et maintenable.

Le projet vise à préserver la connaissance organisationnelle cachée dans les systèmes logiciels en analysant le code, en identifiant les concepts métier, en reconstruisant les processus fonctionnels et en publiant la documentation dans une base de connaissances centralisée telle qu'Outline.

---

## Vision

La connaissance la plus importante d'une organisation est souvent enfouie dans le code.

Avec le temps :

- Les développeurs quittent l'entreprise.
- La documentation devient obsolète.
- Les analystes doivent réinterpréter le système.
- Les équipes perdent du temps à redécouvrir des règles déjà implémentées.

ARGUS a pour mission de rendre cette connaissance visible, compréhensible et durable.

---

## Mission

**Transformer le code source en connaissance durable.**

---

## Objectifs

- Générer automatiquement de la documentation fonctionnelle à partir du code source.
- Maintenir la documentation synchronisée avec l'évolution du logiciel.
- Réduire la dépendance à la connaissance individuelle.
- Créer un glossaire métier cohérent à l'échelle de l'organisation.
- Faciliter le transfert de connaissances entre les équipes de développement, d'analyse et d'affaires.
- Publier automatiquement les résultats dans Outline.
- Préserver la mémoire collective associée aux systèmes logiciels.

---

## Principes de conception

### Le code comme source de vérité

ARGUS considère le code source comme la référence principale pour produire la documentation.

### Documentation vivante

La documentation doit évoluer avec le logiciel et non devenir un artefact statique.

### Traçabilité

Chaque information documentée doit pouvoir être reliée à sa source technique.

### Spécialisation

Chaque agent possède une responsabilité unique et clairement définie.

### Vérification systématique

Aucun contenu n'est publié sans validation.

---

## Architecture générale

```text
ARGUS
│
├── Agent 01 - Orchestrateur
├── Agent 02 - Cartographe
├── Agent 03 - Analyste fonctionnel
├── Agent 04 - Rédacteur
├── Agent 05 - Réviseur
├── Agent 06 - Publicateur Outline
├── Agent 07 - Mise à jour incrémentale
└── Agent 08 - Gardien du glossaire
```

---

## Les agents ARGUS

### Agent 01 - Orchestrateur

#### Rôle

Coordonner l'ensemble du processus documentaire.

#### Responsabilités

- Recevoir les demandes de documentation.
- Déterminer la portée de l'analyse.
- Décomposer le travail.
- Coordonner les agents spécialisés.
- Maintenir le contexte global.
- Vérifier la complétude du processus.

#### Ne doit jamais

- Rédiger la documentation finale.
- Modifier le glossaire.
- Publier dans Outline.

---

### Agent 02 - Cartographe

#### Rôle

Comprendre la structure du système.

#### Responsabilités

- Identifier les modules.
- Détecter les dépendances.
- Cartographier les API.
- Cartographier les flux de données.
- Produire une vue d'ensemble de la solution.

#### Livrables

- Cartographie applicative.
- Inventaire des composants.
- Relations entre modules.

---

### Agent 03 - Analyste fonctionnel

#### Rôle

Transformer la structure technique en compréhension métier.

#### Responsabilités

- Identifier les concepts métier.
- Détecter les cas d'utilisation.
- Reconstruire les processus d'affaires.
- Identifier les règles fonctionnelles.
- Décrire les comportements observés dans le code.

#### Livrables

- Processus métiers.
- Concepts fonctionnels.
- Cas d'utilisation.
- Règles d'affaires détectées.

---

### Agent 04 - Rédacteur

#### Rôle

Créer la documentation destinée aux utilisateurs et aux équipes d'affaires.

#### Responsabilités

- Structurer l'information.
- Produire du contenu clair et cohérent.
- Respecter les standards rédactionnels.
- Générer les documents finaux.

#### Livrables

- Pages fonctionnelles.
- Guides de référence.
- Documentation des modules.

---

### Agent 05 - Réviseur

#### Rôle

Garantir la qualité documentaire.

#### Responsabilités

- Vérifier l'exactitude.
- Vérifier la cohérence.
- Détecter les contradictions.
- Identifier les hallucinations.
- Valider la traçabilité.

#### Livrables

- Rapport de validation.
- Niveau de confiance.
- Liste des corrections demandées.

---

### Agent 06 - Publicateur Outline

#### Rôle

Publier la documentation approuvée.

#### Responsabilités

- Créer les pages.
- Mettre à jour les collections.
- Synchroniser le contenu.
- Maintenir la structure documentaire.

#### Livrables

- Documentation publiée.
- Synchronisation réussie.

---

### Agent 07 - Mise à jour incrémentale

#### Rôle

Maintenir la pertinence de la documentation dans le temps.

#### Responsabilités

- Détecter les changements de code.
- Identifier les impacts documentaires.
- Déclencher des mises à jour ciblées.
- Réduire les régénérations complètes.

#### Livrables

- Rapports d'impact.
- Mises à jour ciblées.
- Historique des modifications.

---

### Agent 08 - Gardien du glossaire

#### Rôle

Préserver la cohérence terminologique.

#### Responsabilités

- Maintenir le vocabulaire métier.
- Détecter les synonymes.
- Identifier les ambiguïtés.
- Standardiser les définitions.

#### Livrables

- Glossaire central.
- Terminologie approuvée.
- Alertes d'incohérence.

---

## Flux d'exécution

```text
Repository Source
        │
        ▼
Agent 01 - Orchestrateur
        │
        ├── Agent 02 - Cartographe
        ├── Agent 03 - Analyste fonctionnel
        └── Agent 08 - Gardien du glossaire
                       │
                       ▼
              Agent 04 - Rédacteur
                       │
                       ▼
               Agent 05 - Réviseur
                       │
                       ▼
        Agent 06 - Publicateur Outline
```

---

## Livrables attendus

ARGUS doit être capable de produire automatiquement :

- Documentation fonctionnelle
- Documentation des modules
- Documentation des processus d'affaires
- Documentation des API
- Documentation des flux de données
- Documentation d'architecture
- Cartographie applicative
- Glossaire métier
- Analyse d'impact
- Rapports de changements
- Documentation de référence pour les équipes d'affaires

---

## Gestion de la connaissance

ARGUS vise à devenir une source de vérité organisationnelle sur les systèmes logiciels.

Le projet ne se limite pas à la génération de documentation. Son objectif est de construire une couche de connaissance capable de :

- Comprendre les systèmes.
- Préserver les règles d'affaires.
- Maintenir la cohérence terminologique.
- Faciliter l'onboarding.
- Réduire la perte de connaissance organisationnelle.
- Soutenir les analyses futures.

---

## Roadmap

### MVP

- Analyse de dépôt Git
- Cartographie des modules
- Analyse fonctionnelle
- Génération Markdown
- Révision automatisée
- Publication dans Outline

### Version 1.0

- Gestion centralisée du glossaire
- Mise à jour incrémentale
- Détection avancée des règles d'affaires
- Historique documentaire

### Version 2.0

- Diagrammes automatiques
- Analyse multi-répertoires
- Analyse inter-systèmes
- Gouvernance documentaire avancée
- Intégration CI/CD complète
- Documentation générée à la demande

---

## Vision à long terme

ARGUS doit devenir la mémoire vivante des systèmes logiciels de l'organisation.

Chaque changement de code, chaque concept métier et chaque règle d'affaires doit pouvoir être découvert, compris, documenté et consulté sans dépendre de la connaissance individuelle d'un développeur ou d'un analyste.

> Le code est la source.