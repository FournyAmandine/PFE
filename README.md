# 🩺 CareTogether - Partager pour soigner 
Site de revente de matériel médical

## 📌 Contexte général
Dans le domaine médical, et plus particulièrement en bandagisterie, orthopédie ou soins à domicile, il est souvent difficile de trouver rapidement du matériel adapté aux besoins spécifiques des patients.

D’un côté, de nombreux particuliers possèdent du matériel médical encore en bon état (fauteuils roulants, béquilles, attelles, lits médicalisés…) qu’ils n’utilisent plus, sans savoir où le vendre, le louer ou le donner.
De l’autre, les professionnels de santé manquent parfois de visibilité sur le matériel disponible sur le marché de seconde main, ce qui complique le conseil aux patients et peut entrainer un manque de suivi pour eux. 

## 🎯 Objectifs du projet

Développer une application web de type marketplace spécialisée dans le matériel médical, permettant de faciliter le réemploi, l’achat, la vente ou la location de matériel médical entre particuliers et professionnels.

### Plus spécifiquement

- Faciliter le réemploi et la disponibilité du matériel médical
- Centraliser les annonces sur une plateforme dédiée
- Mettre en relation particuliers et professionnels de santé
- Offrir un outil d’aide au conseil pour les professionnels
- Concevoir une plateforme :
  - claire,
  - sécurisée,
  - intuitive,
  - accessible à tous
- Mettre en place un CRUD complet conforme aux exigences d’un PFE
- Proposer un design professionnel et qualitatif

## 🛠️ Fonctionnalités principales (CRUD)

### 👤 Gestion des utilisateurs

- Inscription, connexion et déconnexion
- Deux types de comptes :
  - Particulier
  - Professionnel
- Gestion du profil utilisateur :
  - consultation,
  - modification,
  - suppression

---

### 🩺 Gestion du matériel médical

- Ajouter un produit avec :
  - nom,
  - catégorie,
  - description,
  - photos,
  - état (neuf, bon état, à réparer),
  - type (vente / location / don),
  - prix,
  - localisation
- Modifier un produit
- Supprimer un produit
- Consulter les annonces

---

### 🔍 Recherche et filtrage

- Recherche par :
  - nom,
  - catégorie,
  - état,
  - type (vente / location / don),
  - localisation
- Filtrage par :
  - particulier / professionnel
  - proximité géographique

---

### 💬 Messagerie

- Messagerie interne entre utilisateurs
- Messages liés à une annonce
- Historique des conversations

---

### ⭐ Favoris

- Ajouter ou retirer une annonce des favoris
- Consulter la liste des favoris

---

### 🔔 Notifications
- Lorqu'un article mis en favoris est vendu
- Lorqu'un article mis en favoris change de prix
- Lorqu'il y a un message sur le site
- Avertir lorqu'un article est ajouté dans la catégorie recherchée (m'avertir lorqu'il y a en a un nouveau à la vente...)

---

### 🗂️ Gestion des catégories

- CRUD administrateur :
  - création,
  - modification,
  - suppression

---

## 🔒 Exclus du projet

- Paiement en ligne
- Gestion de la livraison
- Logistique avancée
- Certification médicale officielle des produits
- Intelligence artificielle avancée

---

## 👥 Les différents profils

- **Particulier**
  - Publie, recherche, vend, loue ou donne du matériel médical

- **Professionnel**
  - Consulte les annonces
  - Contacte les particuliers
  - Propose des conseils ou des alternatives à leurs clients

- **Administrateur**
  - Gère les catégories
  - Modère les contenus si nécessaire

---


## Personas et scénarios
Afin de mieux comprendre les usages et besoins des différents utilisateurs de la plateforme **CareTogether**, plusieurs personas ont été définis.  
Ces personas permettent d’illustrer des scénarios concrets d’utilisation de l’application, tant du côté des particuliers que des professionnels.

## 👩‍🦽 Marie – Particulier vendeuse de matériel médical

**Âge :** 56 ans  
**Profil :** Aide familiale
**Objectif principal :** Vendre ou donner du matériel médical devenu inutile

### 🧩 Scénario 1 – Publier une annonce de matériel

Suite à une opération du genou de son mari, Marie possède chez elle une paire de béquilles et une attelle qui ne sont plus utilisées. Le matériel est encore en bon état, mais elle ne sait pas où le proposer.

Elle découvre la plateforme **CareTogether** via une bandagisterie locale qui a affiché un QR code dans sa vitrine.

Depuis son ordinateur, Marie crée un compte **particulier**. Une fois connectée, elle accède à son espace personnel et clique sur « Ajouter un produit ».

Elle remplit le formulaire :
- Nom : Attelle de genou réglable
- Catégorie : Orthopédie
- État : Bon état
- Type : Vente
- Prix : 25 €
- Localisation : Namur
- Description : utilisée pendant 2 mois
- Photos : 2 images du produit

Après validation, l’annonce est publiée et visible sur le site. Marie reçoit un email de confirmation.

---

### 🧩 Scénario 2 – Être contactée par un professionnel

Quelques jours plus tard, Marie reçoit une notification par email l’informant qu’un **professionnel** est intéressé par son annonce.

Depuis la messagerie intégrée à CareTogether, elle échange avec Julien, un bandagiste, qui souhaite racheter l’attelle pour un patient. Ils discutent des modalités et conviennent d’un rendez-vous.

Une fois le matériel vendu, Marie modifie le statut de l’annonce en « Vendu ». L’annonce n’apparaît plus dans les résultats publics.

---

## 👨‍⚕️ Julien – Professionnel (bandagiste)

**Âge :** 38 ans  
**Profil :** Bandagiste indépendant  
**Objectif principal :** Trouver rapidement du matériel adapté pour ses patients

### 🧩 Scénario 1 – Rechercher du matériel pour un patient

Julien reçoit un patient qui a besoin d’un fauteuil roulant temporaire. Plutôt que de proposer uniquement du neuf, il souhaite explorer des solutions de seconde main.

Il se connecte à son compte **professionnel** sur CareTogether et effectue une recherche avec les filtres suivants :
- Catégorie : Mobilité
- Type : Location
- Localisation : 30 km autour de Liège

Il consulte plusieurs annonces, compare les états et les prix, puis ouvre la fiche d’un fauteuil roulant proposé par un particulier.

---

### 🧩 Scénario 2 – Contacter un particulier

Depuis la fiche du produit, Julien clique sur « Contacter le vendeur ».  
Le particulier reçoit le message et une discussion s’engage via la messagerie interne.

Grâce à CareTogether, Julien peut rapidement proposer une solution adaptée à son patient, tout en favorisant le réemploi du matériel.

---

### 🧩 Scénario 3 – Publier une annonce professionnelle

Julien souhaite également publier ses propres équipements disponibles en location.

Depuis son espace professionnel, il ajoute une annonce avec :
- Prix professionnel
- Disponibilités
- Informations techniques plus détaillées

Ses annonces sont clairement identifiées comme provenant d’un professionnel, ce qui rassure les utilisateurs.

---

## 👩‍💼 Sophie – Particulier acheteuse / aidante proche

**Âge :** 32 ans  
**Profil :** Employée de bureau, aidante proche de sa grand-mère  
**Objectif principal :** Trouver du matériel médical rapidement et à moindre coût

### 🧩 Scénario 1 – Trouver du matériel adapté

La grand-mère de Sophie sort de l’hôpital et a besoin d’un lit médicalisé pour quelques mois. Sophie n’a aucune idée de où chercher.

Elle arrive sur CareTogether via une recherche Google et utilise la barre de recherche :
- Catégorie : Soins à domicile
- Type : Location
- État : Bon état
- Localisation : Bruxelles

Elle consulte plusieurs fiches produits, lit les descriptions et regarde les photos.

---

### 🧩 Scénario 2 – Contacter et sauvegarder une annonce

Sophie trouve une annonce intéressante mais souhaite la montrer à sa mère avant de se décider.

Elle ajoute l’annonce en **favoris** et utilise la fonction « Partager » pour envoyer le lien par message.

Après validation avec sa famille, elle retourne sur CareTogether et contacte le vendeur via la messagerie.

---

### 🧩 Scénario 3 – Être rassurée par un professionnel

Avant de finaliser la location, Sophie reçoit un message d’un professionnel inscrit sur la plateforme, qui lui confirme que le modèle du lit est adapté à la situation médicale de sa grand-mère.

Rassurée, elle finalise la mise en relation avec le vendeur.

---

## ✅ Apports des scénarios

Ces scénarios montrent que CareTogether :
- facilite la mise en relation entre particuliers et professionnels,
- répond à des besoins concrets et réels,
- valorise le réemploi du matériel médical,
- améliore l’accessibilité au soin,
- propose une expérience utilisateur claire et rassurante.

---

## ⚙️ Contraintes techniques

| Élément | Technologie |
|-------|------------|
| Backend | Laravel |
| Frontend | Blade / Livewire |
| Testing | Pest |
| UI | Tailwind CSS |
| Base de données | MySQL |
| Authentification | Laravel |
| Versioning | GitHub |
| Hébergement | Mutualisé |

---

## 🌐 Site public

### Pages publiques
- Page d’accueil
- Recherche de matériel
- Page détail d’une annonce
- Page À propos
- Page FAQ
- Page Contact
- Mentions légales
- Politique de confidentialité
- Conditions d’utilisation

### Pages d’authentification
- Inscription
- Connexion
- Mot de passe oublié

### Espace utilisateur (particulier)
- Tableau de bord
- Profil utilisateur
- Mes annonces
- Ajouter / modifier une annonce
- Messagerie
- Favoris

### Espace professionnel
- Tableau de bord professionnel
- Profil professionnel
- Mes annonces professionnelles
- Ajouter / modifier une annonce professionnelle
- Messagerie

### Espace administrateur
- Tableau de bord administrateur
