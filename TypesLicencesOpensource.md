# Licence et Conformité Juridique des Logiciels Open Source

La conformité juridique est un aspect critique lorsqu’on utilise, modifie ou redistribue des logiciels open source. Elle permet de **respecter les droits des auteurs**, d’éviter des **litiges** et de garantir que votre projet reste légalement sûr.

## 1. Types de licences open source

Les licences open source définissent **ce que vous pouvez et ne pouvez pas faire** avec un logiciel. Les principales catégories :

### a) Licence GPL (GNU General Public License)

* **Caractéristique principale** : Licence dite "copyleft". Tout logiciel dérivé doit être publié sous la même licence GPL.
* **Exemple concret** : Vous utilisez une bibliothèque GPL pour développer une application commerciale. Si vous redistribuez votre application, vous devez également publier le code source complet sous GPL.
* **Cas pratique** : WordPress est sous GPL. Si vous créez un plugin qui dérive fortement du cœur WordPress, il doit également respecter la GPL.

### b) Licence MIT

* **Caractéristique principale** : Licence très permissive. Elle permet d’utiliser, modifier et redistribuer le code même dans des logiciels propriétaires, avec obligation de conserver le copyright et la licence initiale.
* **Exemple concret** : Vous utilisez une bibliothèque MIT pour votre application mobile. Vous pouvez la distribuer commercialement sans publier votre code source.
* **Cas pratique** : La bibliothèque JavaScript `React` (avant la migration vers MIT) était sous licence MIT, permettant une intégration dans des applications propriétaires.

### c) Licence Apache 2.0

* **Caractéristique principale** : Licence permissive, comme MIT, mais ajoute une **protection contre les brevets**. Elle nécessite de conserver les avis de copyright et de mentionner les modifications apportées.
* **Exemple concret** : Vous intégrez une bibliothèque Apache dans votre application. Vous pouvez distribuer commercialement, mais devez inclure la notice et déclarer toute modification.
* **Cas pratique** : `Apache Hadoop` est sous Apache 2.0. Les entreprises peuvent l’utiliser dans des projets commerciaux tout en respectant la licence.

---

## 2. Vérification des obligations légales selon usage

Avant d’intégrer un logiciel open source, il est important de vérifier les obligations légales liées à votre usage :

* **Redistribution** : Certaines licences (comme GPL) imposent de rendre public votre code source si vous redistribuez le logiciel.
* **Modifications** : Licences Apache ou MIT permettent la modification, mais certaines exigent de notifier les changements.
* **Utilisation commerciale** : Vérifiez si la licence impose des restrictions pour un usage commercial.
* **Compatibilité des licences** : Lorsqu’on combine plusieurs logiciels open source, il faut vérifier que leurs licences sont compatibles.
  **Exemple concret** : Mélanger une bibliothèque GPL avec une bibliothèque MIT dans une même application peut obliger à publier toute l’application sous GPL.

**Outils pour vérifier les licences** :

* `FOSSology` : Analyse automatique des licences.
* `OSS Review Toolkit (ORT)` : Vérifie les obligations légales des composants open source.

---

## 3. Gestion des contributions externes

Lorsqu’un projet open source reçoit des contributions de tiers, il faut gérer les aspects juridiques pour éviter les conflits :

* **Contrats de cession de droits ou CLA (Contributor License Agreement)** : Permettent au projet de sécuriser la propriété intellectuelle et de clarifier les droits d’utilisation.

  * **Exemple concret** : La Fondation Apache demande aux contributeurs de signer un CLA pour éviter tout litige sur la propriété du code.
* **Vérification de la provenance du code** : Éviter l’injection de code provenant d’autres projets avec des licences incompatibles.
* **Historique des contributions** : Maintenir un registre des auteurs pour respecter les obligations de copyright.

---

### ✅ Bonnes pratiques

1. **Documenter toutes les licences utilisées** dans un fichier `LICENSES.txt` ou via un outil de gestion des dépendances.
2. **Analyser la compatibilité des licences** avant de combiner des composants open source.
3. **Former les développeurs** sur les obligations légales de chaque licence.
4. **Mettre en place des CLA** pour les contributions externes.
5. **Auditer régulièrement** le projet pour détecter tout risque juridique.

---


