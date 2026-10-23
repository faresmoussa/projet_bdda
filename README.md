# 🗄️ Projet SGBD - Bases de Données Avancées (BDA) / DBMS Project

> **[FR]** Implémentation d'un Système de Gestion de Bases de Données (SGBD) relationnel simplifié en Java, développé dans le cadre du module de Bases de Données Avancées.  
> **[EN]** Implementation of a simplified relational Database Management System (DBMS) in Java, developed as part of the Advanced Databases course.

---

## 🇫🇷 Version Française

### 📌 Présentation du Projet
Ce projet a pour objectif de concevoir et d'implémenter un moteur de base de données relationnelle en couches modulaires. Il couvre la gestion du stockage physique sur disque jusqu'à la gestion de la mémoire tampon et l'exécution de requêtes.

### 🏗️ Architecture & Composants principaux

- **Gestionnaire Disque (`DiskManager`)** :
  - Allocation, désallocation, lecture et écriture de pages de données sur le disque[cite: 4].
  - Gestion de la persistance des données et de la taille des pages (`pageSize`)[cite: 3, 4].

- **Gestionnaire de Tampon (`BufferManager`)**[cite: 6] :
  - Cache en mémoire vive des pages lues sur le disque.
  - Implémentation des politiques de remplacement de pages pour optimiser les accès I/O.

- **Gestion des Erreurs & Exceptions**[cite: 2, 6] :
  - Exceptions personnalisées (`DiskManagerException`, `BufferManagerException`, `DBMSException`) pour assurer la robustesse de l'application[cite: 6].

### 🚀 Lancement & Utilisation

1. **Prérequis** : Java JDK (17 ou plus récent recommmandé) & Git.
2. **Cloner le projet** :
   ```bash
   git clone <URL_DU_REPOSITORY>
   cd <NOM_DU_DOSSIER>
