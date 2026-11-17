# Développement Efficace et Analyse

Ce dépôt rassemble les travaux pratiques (TP) de **Développement Efficace et Analyse** pour l’année universitaire 2026–2027. Il sert de point d’entrée vers sept dépôts spécialisés, chacun intégré ici comme sous-module Git.

Les TP couvrent la modélisation UML et des structures de données et algorithmes en Java. Les résumés ci-dessous s’appuient sur les consignes, diagrammes, fichiers source et ressources présents dans les sous-modules. Lorsqu’une consigne décrit un travail qui n’apparaît pas dans les fichiers livrés, cela est indiqué comme tel.

## Table des matières

- [Description du projet](#description-du-projet)
- [Organisation du dépôt](#organisation-du-dépôt)
- [Liste des travaux pratiques](#liste-des-travaux-pratiques)
- [Présentation détaillée des TP](#présentation-détaillée-des-tp)
  - [TP 1 — Diagrammes de cas d’utilisation](#tp-1--diagrammes-de-cas-dutilisation)
  - [TP 2 — Listes chaînées](#tp-2--listes-chaînées)
  - [TP 3 — Diagrammes de classes UML](#tp-3--diagrammes-de-classes-uml)
  - [TP 4 — Arbres et piles](#tp-4--arbres-et-piles)
  - [TP 5 — Cas d’utilisation et classes UML](#tp-5--cas-dutilisation-et-classes-uml)
  - [TP 6 — Tris](#tp-6--tris)
  - [TP 7 — Diagrammes de séquence UML](#tp-7--diagrammes-de-séquence-uml)
- [Environnement technique global](#environnement-technique-global)
- [Compétences développées](#compétences-développées)
- [Synthèse et conclusion](#synthèse-et-conclusion)
- [Liens et ressources](#liens-et-ressources)

## Description du projet

Le dépôt a un rôle de **répertoire centralisé** : il référence les dépôts GitHub des TP par des sous-modules et donne une vue d’ensemble de leur contenu. Les consignes portent sur des notions d’analyse et de conception logicielle, la représentation de systèmes en UML, ainsi que l’implémentation et l’étude d’algorithmes et de structures de données.

Le contexte visible dans les consignes est celui d’exercices pédagogiques. L’établissement et le cours exacts ne sont pas précisés dans les fichiers consultés. Les dépôts secondaires restent les sources de référence pour les consignes, diagrammes, exemples et codes de chaque TP.

## Organisation du dépôt

À la racine se trouvent le présent README, le fichier `.gitmodules` et sept sous-modules :

| Dossier | Contenu principal |
| --- | --- |
| [`tp1-cas-utilisation-uml_r303_26-27/`](./tp1-cas-utilisation-uml_r303_26-27/) | Consignes, diagrammes et images sur les cas d’utilisation. |
| [`tp2-liste-chainees_r302_26-27/`](./tp2-liste-chainees_r302_26-27/) | Implémentation Java d’une liste simplement chaînée. |
| [`tp3-diagrammes-classe-uml_r303_26-27/`](./tp3-diagrammes-classe-uml_r303_26-27/) | Diagrammes de classes, consignes, PDF et exemples Java de gestion de bibliothèque. |
| [`tp4-arbres-piles_r303_26-27/`](./tp4-arbres-piles_r303_26-27/) | Consignes sur les arbres et les piles, avec une implémentation Java d’arbre générique. |
| [`tp5-diagrammes-cas_util-et-classe-uml_r303_26-27/`](./tp5-diagrammes-cas_util-et-classe-uml_r303_26-27/) | Modèles UML et illustrations pour plusieurs études de cas. |
| [`tp6-tris_r302_26-27/`](./tp6-tris_r302_26-27/) | Implémentations Java de tri à bulles et de QuickSort. |
| [`tp7-diagrammes-sequences-uml_r303_26-27/`](./tp7-diagrammes-sequences-uml_r303_26-27/) | Consignes et diagrammes UML de séquence autour d’un contrôle d’accès. |

Chaque sous-module possède son propre historique et son propre dépôt distant. Il faut donc cloner les sous-modules pour disposer de leur contenu lors d’un nouveau clonage :

```bash
git clone --recurse-submodules https://github.com/SISE-Aboubakar-24027352/r302_303-dev_efficace_et_analyse-26_27.git
```

Depuis une copie déjà clonée sans sous-modules :

```bash
git submodule update --init --recursive
```

## Liste des travaux pratiques

| TP | Intitulé | Contenu résumé | Technologies principales | Dépôt |
| --- | --- | --- | --- | --- |
| 1 | Diagrammes de cas d’utilisation | Modélisation de quatre systèmes : billetterie ferroviaire, ascenseur, livraison de repas et guichet bancaire. | UML, fichiers `.puml`, images PNG | [Dépôt TP1](https://github.com/SISE-Aboubakar-24027352/tp1-cas-utilisation-uml_r303_26-27) |
| 2 | Listes chaînées | Liste simplement chaînée d’entiers et opérations de base, avec un programme de démonstration. | Java, classes imbriquées, maillons chaînés | [Dépôt TP2](https://github.com/SISE-Aboubakar-24027352/tp2-liste-chainees_r302_26-27) |
| 3 | Diagrammes de classes UML | Relations UML et conception d’un modèle de gestion des emprunts d’une bibliothèque ; exemples Java de classes. | UML, PlantUML (`.puml`), Java, PDF et PNG | [Dépôt TP3](https://github.com/SISE-Aboubakar-24027352/tp3-diagrammes-classe-uml_r303_26-27) |
| 4 | Arbres et piles | Arbres génériques, parcours, représentation d’un DOM, expressions postfixées et piles dans les consignes ; code livré centré sur les arbres. | Java, génériques, listes d’enfants | [Dépôt TP4](https://github.com/SISE-Aboubakar-24027352/tp4-arbres-piles_r303_26-27) |
| 5 | Cas d’utilisation et classes UML | Modèles de classes pour un réseau ferroviaire et une location de bungalows ; un troisième exercice d’inscription à l’IUT est décrit dans les consignes. | UML, PlantUML (`.puml`), images PNG | [Dépôt TP5](https://github.com/SISE-Aboubakar-24027352/tp5-diagrammes-cas_util-et-classe-uml_r303_26-27) |
| 6 | Tris | Tri à bulles sur tableau d’entiers et QuickSort générique sur une file, avec exemples de lancement. | Java, `Comparator`, `Queue`, `LinkedList` | [Dépôt TP6](https://github.com/SISE-Aboubakar-24027352/tp6-tris_r302_26-27) |
| 7 | Diagrammes de séquence UML | Scénarios d’un contrôle d’accès à un bâtiment, avec un diagramme de classes initial et une séquence nominale. | UML, PlantUML (`.puml`), images PNG | [Dépôt TP7](https://github.com/SISE-Aboubakar-24027352/tp7-diagrammes-sequences-uml_r303_26-27) |

## Présentation détaillée des TP

### TP 1 — Diagrammes de cas d’utilisation

**Objectif pédagogique.** Identifier les acteurs et les fonctionnalités d’un système à partir d’un énoncé, puis représenter les interactions et certains scénarios en UML.

**Contenu et réalisations présentes.** Le document [`tp1.md`](./tp1-cas-utilisation-uml_r303_26-27/tp1.md) présente les notions d’acteur, de cas d’utilisation et de relations. Quatre études de cas sont accompagnées de sources `.puml` et de diagrammes PNG :

1. **Réservation de trains** : achat de billet ou d’abonnement, actualisation des tarifs et situations d’erreur.
2. **Contrôle d’un ascenseur** : appels depuis les boutons intérieur et extérieur, affichage, déplacement et scénario textuel « Choisir étage ».
3. **Portail de livraison de repas** : clients individuels ou groupes, choix de menus, régime alimentaire, subventions, cuisine industrielle, livraison et facturation.
4. **Guichet automatique bancaire** : retraits, consultation du solde, dépôts, authentification, sécurisation et rechargement du distributeur. Le README du TP fournit aussi des descriptions textuelles de cas d’utilisation.

Les diagrammes mobilisent les acteurs, les frontières de système, les associations, la généralisation et les relations `<<include>>` et `<<extend>>`. Les descriptions et diagrammes sont des travaux d’analyse et de modélisation ; aucun programme applicatif n’est présent dans ce sous-module.

**Technologies et exécution.** Les sources sont des fichiers `.puml` accompagnés d’illustrations PNG. La consigne mentionne StarUML ; aucun fichier de configuration, commande de génération ou environnement d’exécution n’est fourni. Le logiciel utilisé pour produire ou rendre chaque image n’est pas uniformément indiqué.

**Liens.** [Dépôt GitHub](https://github.com/SISE-Aboubakar-24027352/tp1-cas-utilisation-uml_r303_26-27) · [Consignes et résultats](./tp1-cas-utilisation-uml_r303_26-27/tp1.md)

### TP 2 — Listes chaînées

**Objectif pédagogique.** Comprendre les opérations fondamentales sur une liste simplement chaînée et les mettre en œuvre en Java.

**Contenu et réalisations présentes.** [`SinglyListClass.java`](./tp2-liste-chainees_r302_26-27/src/exo1/SinglyListClass.java) implémente une liste d’`Integer` sans sentinelle. Elle fournit `size()` (calcul récursif), `isEmpty()`, `first()`, `last()`, `addFirst()`, `addLast()`, `removeFirst()` et `toString()`. Le type de maillon `Node` est une classe interne privée statique. Les accesseurs qui consultent ou retirent un élément d’une liste vide renvoient `null`.

[`Main.java`](./tp2-liste-chainees_r302_26-27/src/exo1/Main.java) exerce ces opérations avec des exemples d’ajout, de consultation et de retrait, y compris sur une liste vide. Les autres sujets du document pédagogique — liste doublement chaînée, liste circulaire, génériques, inversion et échange de nœuds — sont des extensions proposées ; leur implémentation n’est pas présente dans les sources relevées.

**Technologies et exécution.** Java, sans bibliothèque externe ni outil de build déclaré. Depuis le dossier du TP, avec un JDK installé :

```bash
mkdir -p out
javac -d out src/exo1/*.java
java -cp out exo1.Main
```

Les vérifications sont des sorties comparées visuellement à des résultats attendus dans `Main`; aucun framework de test n’est configuré.

**Liens.** [Dépôt GitHub](https://github.com/SISE-Aboubakar-24027352/tp2-liste-chainees_r302_26-27) · [Consignes](./tp2-liste-chainees_r302_26-27/README.md) · [Implémentation](./tp2-liste-chainees_r302_26-27/src/exo1/SinglyListClass.java)

### TP 3 — Diagrammes de classes UML

**Objectif pédagogique.** Représenter la structure statique d’un système avec des classes, attributs, relations, multiplicités, spécialisations et dépendances, puis relier un diagramme à du code.

**Contenu et réalisations présentes.** Le premier exercice traite plusieurs exemples de relations UML : articles et commandes, compagnies et vols, mariage, dépendance entre `Document` et `Imprimante`, composition entre répertoire et fichiers, murs partagés entre pièces, association, agrégation, composition, héritage, dépendance et réalisation. Les diagrammes sont fournis en `.puml` et en images.

Le second exercice modélise une **bibliothèque universitaire** : adhérents (étudiants ou professeurs), documents (journaux ou volumes), catégories de volumes, emprunts et bibliothèque. Le modèle représente notamment la limite de quatre emprunts simultanés et l’emprunt d’un volume par une seule personne à la fois. Les fichiers [`Adherent.java`](./tp3-diagrammes-classe-uml_r303_26-27/exo2/Adherent.java), [`Emprunt.java`](./tp3-diagrammes-classe-uml_r303_26-27/exo2/Emprunt.java) et [`Volume.java`](./tp3-diagrammes-classe-uml_r303_26-27/exo2/Volume.java) illustrent l’inscription, la vérification de disponibilité, les dates de restitution et la libération d’un volume.

Le dépôt comprend aussi le sujet PDF [`TP3-ClassDiag.pdf`](./tp3-diagrammes-classe-uml_r303_26-27/TP3-ClassDiag.pdf). Aucun programme principal ni jeu de tests automatisés n’est fourni pour les classes de bibliothèque.

**Technologies et exécution.** Diagrammes UML en syntaxe PlantUML, images PNG, PDF et Java. Aucun outil de build n’est déclaré. Les sources Java de l’exercice bibliothèque peuvent être compilées depuis le dossier du TP :

```bash
mkdir -p out
javac -d out exo2/*.java
```

Cette commande compile les classes ; aucun point d’entrée exécutable ou test n’est fourni. La source utilise `List.copyOf`, disponible à partir de Java 10.

**Liens.** [Dépôt GitHub](https://github.com/SISE-Aboubakar-24027352/tp3-diagrammes-classe-uml_r303_26-27) · [Consignes](./tp3-diagrammes-classe-uml_r303_26-27/tp3.md) · [Modèle de bibliothèque](./tp3-diagrammes-classe-uml_r303_26-27/exo2/exo2.puml)

### TP 4 — Arbres et piles

**Objectif pédagogique.** Étudier les arbres n-aires et leurs parcours, leur application à un DOM ou à une expression arithmétique, puis aborder la pile et l’évaluation d’expressions en notation postfixée.

**Contenu et réalisations présentes.** [`ArbreNode.java`](./tp4-arbres-piles_r303_26-27/src/exo1/ArbreNode.java) définit un nœud générique avec parent et liste d’enfants, ainsi que des méthodes pour consulter/modifier son contenu, repérer racine et feuille, parcourir l’arbre en préfixe et produire une représentation textuelle indentée. [`Main.java`](./tp4-arbres-piles_r303_26-27/src/exo1/Main.java) vise à construire un arbre représentant un document HTML simple.

Les consignes abordent également les parcours postfixés, les arbres d’expressions, la création d’une API d’arbre, une pile générique `MaPile<T>` et l’évaluation d’expressions en NPI. Aucune implémentation de pile ni d’évaluateur NPI n’est présente dans les fichiers source inventoriés.

**Point d’attention sur l’exécution.** Dans l’état des sources, les noms de méthodes appelés dans `Main.java` (`ajouterEnfant`) ne correspondent pas aux noms déclarés dans `ArbreNode.java` (`ajouterenfants`). L’appel utilisé pour retirer des enfants dans `ArbreNode` affecte également le parent au lieu de le détacher. Le programme ne peut donc pas être compilé et exécuté tel quel ; les sources ne sont pas modifiées par ce dépôt principal.

**Technologies.** Java et génériques. La méthode `String.repeat` présente dans la représentation textuelle nécessite Java 11 ou ultérieur. Aucun outil de build ni test automatisé n’est déclaré.

**Liens.** [Dépôt GitHub](https://github.com/SISE-Aboubakar-24027352/tp4-arbres-piles_r303_26-27) · [Consignes](./tp4-arbres-piles_r303_26-27/README.md) · [Nœud d’arbre](./tp4-arbres-piles_r303_26-27/src/exo1/ArbreNode.java)

### TP 5 — Cas d’utilisation et classes UML

**Objectif pédagogique.** Analyser des scénarios métier et construire des modèles statiques sous forme de diagrammes de classes UML.

**Contenu et réalisations présentes.** Le dépôt fournit deux diagrammes de classes en `.puml`, accompagnés d’images :

- **Simulation d’un réseau ferroviaire** : lignes, gares, trains, capteurs et barrières ; les associations représentent notamment les gares traversées, les gares de départ et d’arrivée et les capteurs associés aux barrières.
- **Location de bungalows** : clients, réservations, bungalows et types, tarifs, paiements, états des lieux et réparations.

Le README du TP décrit un troisième exercice sur les inscriptions à l’IUT et les consignes demandent plusieurs vues UML. Toutefois, aucun diagramme correspondant à ce troisième exercice n’apparaît parmi les fichiers `.puml` et illustrations inventoriés. Malgré l’intitulé du dépôt, les fichiers de modélisation disponibles sont des diagrammes de classes ; aucun diagramme de cas d’utilisation dédié ni code applicatif n’a été identifié.

**Technologies et exécution.** Sources PlantUML et images PNG. Pas de langage de programmation, dépendance, commande de lancement ou test applicable au contenu livré. Aucun outil de rendu n’est spécifié.

**Liens.** [Dépôt GitHub](https://github.com/SISE-Aboubakar-24027352/tp5-diagrammes-cas_util-et-classe-uml_r303_26-27) · [Consignes et diagrammes](./tp5-diagrammes-cas_util-et-classe-uml_r303_26-27/tp5.md) · [Dossier des sources UML](./tp5-diagrammes-cas_util-et-classe-uml_r303_26-27/exos/)

### TP 6 — Tris

**Objectif pédagogique.** Implémenter et examiner des algorithmes de tri, puis étudier les choix de pivot et les mesures de performance proposés dans les consignes.

**Contenu et réalisations présentes.**

- [`BubbleSort.java`](./tp6-tris_r302_26-27/src/exo1/BubbleSort.java) trie en place un tableau `int[]` avec des boucles imbriquées et échange les éléments adjacents lorsqu’ils sont dans le mauvais ordre. Un exemple d’exécution est fourni dans `main`.
- [`QuickSort.java`](./tp6-tris_r302_26-27/src/exo2/QuickSort.java) fournit un tri générique utilisant `Comparator<K>` et l’interface `Queue<K>`. Le partitionnement distribue les éléments dans trois files (`lesser`, `equal`, `greater`), puis les sous-files sont triées récursivement et concaténées. L’exemple utilise `LinkedList<Integer>` et l’ordre naturel.

La consigne du tri à bulles évoque une liste doublement chaînée, tandis que le code présent traite un tableau. Elle propose pour QuickSort un travail sur `ArrayList`, puis des mesures, un CSV, un pivot randomisé et la médiane-de-trois ; l’implémentation livrée utilise plutôt `Queue` et ne contient pas ces extensions ni le programme de benchmark. Le fichier [`PseudoCode.md`](./tp6-tris_r302_26-27/src/exo2/PseudoCode.md) rappelle un algorithme de partitionnement en files.

**Technologies et exécution.** Java standard (`Comparator`, `Queue`, `LinkedList`, `Arrays`), sans dépendance externe ni outil de build déclaré. Depuis le dossier du TP :

```bash
mkdir -p out
javac -d out src/exo1/BubbleSort.java src/exo2/QuickSort.java
java -cp out exo1.BubbleSort
java -cp out exo2.QuickSort
```

Ces programmes affichent des exemples de tri ; aucun framework de test automatisé n’est configuré.

**Liens.** [Dépôt GitHub](https://github.com/SISE-Aboubakar-24027352/tp6-tris_r302_26-27) · [Consignes](./tp6-tris_r302_26-27/README.md) · [QuickSort](./tp6-tris_r302_26-27/src/exo2/QuickSort.java)

### TP 7 — Diagrammes de séquence UML

**Objectif pédagogique.** Décrire temporellement les échanges entre acteurs et objets pour des scénarios d’un cas d’utilisation, puis faire évoluer le modèle de classes en fonction des messages.

**Contenu et réalisations présentes.** Le cas étudié est un système de contrôle d’accès à un bâtiment : saisie d’un code à quatre chiffres avec une limite de cinq secondes, vérification en base de données, ouverture de porte et délai de vingt secondes, voyants, alarme et archivage des tentatives. Le dépôt fournit un diagramme de classes initial et un diagramme de séquence nominal dans les fichiers `.puml`, ainsi que des images correspondantes.

Les consignes couvrent aussi les scénarios d’échec et demandent de compléter les diagrammes au fil de l’analyse. Dans les fichiers livrés, seul le scénario nominal est représenté en séquence ; les autres scénarios ne sont pas identifiés comme diagrammes réalisés. Aucun code applicatif ni test n’est présent.

**Technologies et exécution.** Modèles UML en syntaxe PlantUML et illustrations PNG. Aucun environnement d’exécution, dépendance ou commande de rendu n’est spécifié.

**Liens.** [Dépôt GitHub](https://github.com/SISE-Aboubakar-24027352/tp7-diagrammes-sequences-uml_r303_26-27) · [Consignes](./tp7-diagrammes-sequences-uml_r303_26-27/tp7.md) · [Sources des diagrammes](./tp7-diagrammes-sequences-uml_r303_26-27/exos/)

## Environnement technique global

| Domaine | Technologies et outils relevés |
| --- | --- |
| Langages | Java pour les structures de données et algorithmes des TP 2, 3, 4 et 6. Les diagrammes textuels sont écrits en syntaxe PlantUML (`.puml`). |
| Bibliothèques Java | Les sources examinées utilisent principalement l’API standard du JDK : collections (`List`, `ArrayList`, `Queue`, `LinkedList`), `Comparator`, `Arrays` et `java.time.LocalDate`. |
| Outils UML et formats | Fichiers `.puml`, illustrations PNG et un document PDF. StarUML est cité dans les consignes du TP 1 ; aucun outil de génération standard pour l’ensemble des diagrammes n’est spécifié. |
| Gestion des dépôts | Git et sous-modules Git ; les remotes des sept dépôts sont déclarés dans `.gitmodules`. |
| Build et tests | Aucun fichier de build ou configuration de tests automatisés n’a été identifié dans les sous-modules. Les exemples Java comportent des méthodes `main` avec sorties console. |
| Environnement Java | La version du JDK n’est pas définie par une configuration de projet. Le code du TP 4 utilise `String.repeat` (Java 11+) et le code du TP 3 utilise `List.copyOf` (Java 10+). |

## Compétences développées

- **Analyse fonctionnelle** : délimiter le système, identifier ses acteurs, ses services, ses scénarios nominaux et alternatifs.
- **Modélisation UML** : construire des diagrammes de cas d’utilisation, de classes et de séquence ; exprimer relations, multiplicités, responsabilités et ordre des interactions.
- **Programmation Java** : utiliser classes, classes internes, génériques, récursivité, collections, comparateurs et API de dates.
- **Structures de données** : manipuler listes chaînées, files et arbres n-aires ; raisonner sur les liens entre nœuds.
- **Algorithmique** : parcourir et représenter un arbre, partitionner des données et implémenter des tris.
- **Vérification** : confronter les résultats affichés à des exemples attendus et repérer les écarts entre consignes et implémentations.
- **Organisation du travail** : naviguer entre dépôts Git référencés comme sous-modules et consulter leurs fichiers de conception et de code.

## Synthèse et conclusion

L’ensemble suit deux axes complémentaires : la **conception et l’analyse UML** (TP 1, 3, 5 et 7) et la **programmation de structures de données et algorithmes** (TP 2, 4 et 6). La progression des sujets UML va de l’identification des fonctionnalités et acteurs vers la modélisation des classes, puis la représentation temporelle des interactions. Les TP Java passent des opérations de listes à l’arbre et aux tris.

Les fichiers livrés illustrent plusieurs de ces notions avec des diagrammes, des exemples Java et des sorties console. Ils ne couvrent toutefois pas toujours toutes les extensions proposées dans les consignes ; les écarts et points de compilation visibles sont précisés dans les sections concernées. Pour le détail et l’historique de chaque travail, consulter son dépôt secondaire.

## Liens et ressources

### Dépôts des TP

1. [TP 1 — Cas d’utilisation UML](https://github.com/SISE-Aboubakar-24027352/tp1-cas-utilisation-uml_r303_26-27)
2. [TP 2 — Listes chaînées](https://github.com/SISE-Aboubakar-24027352/tp2-liste-chainees_r302_26-27)
3. [TP 3 — Diagrammes de classes UML](https://github.com/SISE-Aboubakar-24027352/tp3-diagrammes-classe-uml_r303_26-27)
4. [TP 4 — Arbres et piles](https://github.com/SISE-Aboubakar-24027352/tp4-arbres-piles_r303_26-27)
5. [TP 5 — Cas d’utilisation et diagrammes de classes UML](https://github.com/SISE-Aboubakar-24027352/tp5-diagrammes-cas_util-et-classe-uml_r303_26-27)
6. [TP 6 — Tris](https://github.com/SISE-Aboubakar-24027352/tp6-tris_r302_26-27)
7. [TP 7 — Diagrammes de séquence UML](https://github.com/SISE-Aboubakar-24027352/tp7-diagrammes-sequences-uml_r303_26-27)

### Références techniques mentionnées dans les consignes

- [Documentation Java](https://docs.oracle.com/en/java/)
- [Tutoriel de Dévelopement Java](https://www.jmdoudoux.fr/accueil_java.htm)
- [Tutoriel Java — classes imbriquées](https://docs.oracle.com/javase/tutorial/java/javaOO/nested.html), cité dans les consignes du TP 2.
- Documentation Java de `List` et `LinkedList`, recommandée dans les consignes du TP 2.
- Documentation Java de `Stack<T>`, recommandée dans les consignes du TP 4.