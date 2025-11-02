# 🏪 Système de Gestion de Stock - Magasin Management

[![Demo](https://img.shields.io/badge/Demo-Live-success?style=for-the-badge&logo=vercel)](https://magasin-management.vercel.app)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

> 🌐 **Démo en ligne :** [magasin-management.vercel.app](https://magasin-management.vercel.app)

## 📋 Table des Matières

- [Démo en ligne](#-démo-en-ligne)
- [Vue d'ensemble](#vue-densemble)
- [Fonctionnalités principales](#fonctionnalités-principales)
- [Technologies utilisées](#technologies-utilisées)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Configuration](#configuration)
- [Utilisation](#utilisation)
- [Structure du projet](#structure-du-projet)
- [API Documentation](#api-documentation)
- [Rôles et permissions](#rôles-et-permissions)
- [Base de données](#base-de-données)
- [Déploiement](#déploiement)
- [Contribution](#contribution)
- [Auteur](#auteur)


---

## 🌐 Démo en ligne

### 🚀 Essayez l'application maintenant !

**URL de démonstration :** [https://magasin-management.vercel.app](https://magasin-management.vercel.app)

### 🔑 Comptes de test

Connectez-vous avec l'un de ces comptes pour explorer les différents niveaux d'accès :

| Rôle | Email | Mot de passe | Permissions |
|------|-------|--------------|-------------|
| **👑 Admin** | `admin@inventory.com` | `Admin123!` | Accès complet (gestion utilisateurs, analytics, configuration) |
| **⚙️ Manager** | `manager@inventory.com` | `Manager123!` | Gestion complète des stocks et rapports |
| **👤 User** | `user@inventory.com` | `User123!` | Consultation et enregistrement de mouvements |

> 💡 **Astuce :** Testez chaque compte pour voir les différentes interfaces et permissions !

---

## 🎯 Vue d'ensemble

Le **Système de Gestion de Stock** est une application web complète et moderne conçue pour gérer efficacement l'inventaire d'une organisation. Cette solution offre une plateforme centralisée pour le suivi, la gestion et l'analyse des stocks en temps réel.

### Objectifs du projet

- **Optimiser la gestion des stocks** : Suivre précisément les quantités, catégories et statuts des articles
- **Traçabilité complète** : Enregistrer tous les mouvements (entrées/sorties) avec historique détaillé
- **Prévenir les ruptures** : Alertes automatiques pour les articles en faible stock
- **Sécurité renforcée** : Système d'authentification robuste avec gestion des rôles
- **Analyses approfondies** : Tableaux de bord et rapports pour des décisions éclairées

### Cas d'utilisation

Ce système est particulièrement adapté pour :
- Les ateliers industriels (gestion d'outils et pièces détachées)
- Les magasins et entrepôts
- Les services de maintenance
- Toute organisation nécessitant un suivi précis de son inventaire

---

## ✨ Fonctionnalités principales

### 🔐 Authentification et sécurité
- **Inscription et connexion sécurisées** avec hashage des mots de passe
- **Vérification d'email** pour validation des comptes
- **Réinitialisation de mot de passe** via email
- **Sessions sécurisées** avec JWT (JSON Web Tokens)
- **Système d'invitations** pour l'ajout de nouveaux utilisateurs

### 📦 Gestion des stocks
- **Ajout/Modification/Suppression** d'articles
- **Catégorisation** flexible des articles
- **Suivi des quantités** en temps réel
- **Statuts automatiques** : En stock, Stock faible, Rupture
- **Dates de retour prévues** pour les articles empruntés
- **Import/Export** de données (Excel, CSV)

### 📊 Suivi des mouvements
- **Journal complet** de tous les mouvements (entrées/sorties)
- **Traçabilité** : qui, quoi, quand, combien
- **Filtrage avancé** par date, type, utilisateur
- **Historique détaillé** par article

### 👥 Gestion des utilisateurs
- **Trois niveaux de rôles** : Admin, Manager, User
- **Gestion des permissions** granulaire
- **Profils utilisateurs** personnalisables
- **Invitations par email** pour nouveaux membres

### 📈 Tableaux de bord et rapports
- **Dashboard analytique** avec métriques clés
- **Graphiques interactifs** (distribution par catégorie, tendances)
- **Rapports exportables** en Excel/PDF
- **Alertes visuelles** pour stock faible
- **Calendrier** pour planification des retours

### 🌍 Fonctionnalités additionnelles
- **Multilingue** (Français, Anglais, Arabe)
- **Mode sombre/clair** pour le confort visuel
- **Recherche globale** instantanée
- **Interface responsive** (mobile, tablette, desktop)
- **PWA** (Progressive Web App) - installation possible

---

## 🛠️ Technologies utilisées

### Frontend
- **Next.js 14** - Framework React pour applications fullstack
- **React 18** - Bibliothèque UI moderne
- **TypeScript** - JavaScript typé pour plus de fiabilité
- **Tailwind CSS** - Framework CSS utilitaire
- **Shadcn/UI** - Composants UI accessibles et personnalisables
- **Lucide React** - Icônes modernes
- **React Hook Form** - Gestion des formulaires
- **Zod** - Validation de schémas
- **Recharts** - Graphiques et visualisations
- **FullCalendar** - Gestion du calendrier

### Backend
- **Next.js API Routes** - Endpoints API RESTful
- **Prisma ORM** - Gestion de base de données typée
- **PostgreSQL** - Base de données relationnelle
- **Jose** - Gestion des JWT
- **Bcrypt** - Hashage sécurisé des mots de passe

### Outils et librairies
- **ExcelJS** - Export/Import Excel
- **date-fns** - Manipulation de dates
- **Sonner** - Notifications toast
- **next-themes** - Gestion des thèmes
- **next-pwa** - Support Progressive Web App

### Déploiement
- **Vercel** - Plateforme de déploiement optimisée pour Next.js
- **Vercel Speed Insights** - Monitoring des performances

---

## 📋 Prérequis

Avant de commencer, assurez-vous d'avoir installé :

- **Node.js** version 18.x ou supérieure
- **npm** ou **pnpm** (gestionnaire de paquets)
- **PostgreSQL** version 14 ou supérieure
- **Git** pour le contrôle de version

---

## 🚀 Installation

### 1. Cloner le dépôt

```bash
git clone https://github.com/Ilykao171/magasin-management.git
cd magasin-management
```

### 2. Installer les dépendances

Avec npm :
```bash
npm install
```

Ou avec pnpm (recommandé) :
```bash
pnpm install
```

### 3. Configuration de la base de données

Créez une base de données PostgreSQL :
```sql
CREATE DATABASE magasin_management;
```

### 4. Variables d'environnement

Créez un fichier `.env` à la racine du projet :

```env
# Database
DATABASE_URL="postgresql://username:password@localhost:5432/magasin_management"

# JWT Secret (générez une clé aléatoire sécurisée)
JWT_SECRET="votre_secret_jwt_tres_securise_ici"

# Email Configuration (pour la réinitialisation de mot de passe)
EMAIL_SERVER_HOST="smtp.gmail.com"
EMAIL_SERVER_PORT="587"
EMAIL_FROM="noreply@votre-domaine.com"
EMAIL_SERVER_USER="votre-email@gmail.com"
EMAIL_SERVER_PASSWORD="votre-mot-de-passe-application"

# Application URL
NEXT_PUBLIC_APP_URL="http://localhost:3000"
```

### 5. Initialiser la base de données

Appliquez les migrations Prisma :
```bash
npx prisma migrate deploy
```

Générez le client Prisma :
```bash
npx prisma generate
```

### 6. (Optionnel) Données de démonstration

Pour ajouter des données de test :
```bash
npm run seed
```

Cela créera les comptes de démonstration mentionnés dans la section [Démo en ligne](#-démo-en-ligne).

---

## ▶️ Utilisation

### Démarrage en développement

```bash
npm run dev
```

L'application sera accessible sur [http://localhost:3000](http://localhost:3000)

> � **Vous voulez juste tester l'application ?** Rendez-vous sur la [démo en ligne](https://magasin-management.vercel.app) !

### Build de production

```bash
npm run build
npm run start
```

### Commandes utiles

- `npm run lint` - Vérifier le code avec ESLint
- `npx prisma studio` - Interface graphique pour la base de données
- `npx prisma migrate dev` - Créer une nouvelle migration

---

## 📁 Structure du projet

```
magasin-management/
├── app/                          # Application Next.js (App Router)
│   ├── api/                      # Routes API backend
│   │   ├── analytics/            # Endpoints d'analyse
│   │   ├── auth/                 # Authentification
│   │   ├── calendar/             # Gestion du calendrier
│   │   ├── inventory/            # Gestion des stocks
│   │   ├── movements/            # Journal des mouvements
│   │   └── users/                # Gestion des utilisateurs
│   ├── admin/                    # Pages d'administration
│   ├── all-stock/                # Vue complète des stocks
│   ├── calendar/                 # Interface calendrier
│   ├── login/                    # Page de connexion
│   ├── register/                 # Inscription
│   ├── manage-stock/             # Gestion des stocks
│   ├── movement-log/             # Historique des mouvements
│   ├── reports/                  # Rapports et analyses
│   ├── settings/                 # Paramètres utilisateur
│   └── layout.tsx                # Layout principal
├── components/                   # Composants React réutilisables
│   ├── ui/                       # Composants UI de base (Shadcn)
│   ├── sidebar.tsx               # Barre latérale de navigation
│   ├── theme-toggle.tsx          # Sélecteur de thème
│   ├── protected-route.tsx       # Protection des routes
│   └── ...
├── context/                      # Contextes React
│   ├── auth-context.tsx          # État d'authentification global
│   ├── inventory-context.tsx     # État de l'inventaire
│   ├── language-context.tsx      # Gestion multilingue
│   └── notification-context.tsx  # Système de notifications
├── hooks/                        # Hooks personnalisés
├── lib/                          # Utilitaires et configurations
│   ├── auth.ts                   # Logique d'authentification
│   ├── prisma.ts                 # Configuration Prisma
│   └── utils.ts                  # Fonctions utilitaires
├── prisma/                       # Configuration base de données
│   ├── schema.prisma             # Schéma de la base
│   └── migrations/               # Historique des migrations
├── public/                       # Fichiers statiques
│   ├── locales/                  # Fichiers de traduction
│   └── icons/                    # Icônes PWA
├── utils/                        # Utilitaires métier
│   ├── excel-export.ts           # Export Excel
│   ├── file-parser.ts            # Parser de fichiers
│   └── import-helpers.ts         # Helpers d'import
└── ...
```

---

## 🔌 API Documentation

### Authentification

#### POST `/api/auth/register`
Inscription d'un nouvel utilisateur

**Body:**
```json
{
  "email": "user@example.com",
  "username": "utilisateur",
  "password": "MotDePasse123!",
  "firstName": "Prénom",
  "lastName": "Nom",
  "invitationToken": "token-invitation-optionnel"
}
```

#### POST `/api/auth/login`
Connexion d'un utilisateur

**Body:**
```json
{
  "email": "user@example.com",
  "password": "MotDePasse123!"
}
```

#### POST `/api/auth/logout`
Déconnexion

#### POST `/api/auth/forgot-password`
Demande de réinitialisation de mot de passe

**Body:**
```json
{
  "email": "user@example.com"
}
```

### Inventaire

#### GET `/api/inventory`
Récupérer tous les articles
- Query params: `category`, `status`, `search`

#### POST `/api/inventory`
Ajouter un nouvel article

**Body:**
```json
{
  "name": "Nom de l'article",
  "category": "Outillage",
  "quantity": 10,
  "expectedReturnDate": "2025-12-31"
}
```

#### PUT `/api/inventory/[id]`
Mettre à jour un article

#### DELETE `/api/inventory/[id]`
Supprimer un article

### Mouvements

#### GET `/api/movements`
Récupérer l'historique des mouvements
- Query params: `startDate`, `endDate`, `type`, `itemId`

#### POST `/api/movements`
Enregistrer un nouveau mouvement

**Body:**
```json
{
  "type": "Sortie",
  "itemId": "item-id",
  "quantity": 2,
  "handledBy": "user-id",
  "expectedReturnDate": "2025-11-15"
}
```

### Analytics

#### GET `/api/analytics/dashboard`
Métriques du tableau de bord

**Response:**
```json
{
  "totalItems": 150,
  "lowStockItems": 12,
  "totalMovements": 450,
  "categoryDistribution": [...],
  "recentActivity": [...]
}
```

---

## 👤 Rôles et permissions

### 🔴 Admin (Administrateur)
- **Accès complet** à toutes les fonctionnalités
- Gestion des utilisateurs (création, modification, suppression)
- Gestion des invitations
- Configuration système
- Accès aux analytics avancées
- Export de toutes les données

### 🟡 Manager (Gestionnaire)
- Gestion complète de l'inventaire
- Consultation et création de rapports
- Validation des mouvements
- Gestion des articles (ajout, modification, suppression)
- Consultation de l'historique complet
- Export de données

### 🟢 User (Utilisateur standard)
- Consultation de l'inventaire
- Enregistrement de sorties/entrées d'articles
- Consultation de l'historique de ses propres mouvements
- Mise à jour de son profil

---

## 💾 Base de données

### Schéma Prisma

#### User (Utilisateur)
```prisma
model User {
  id              String    @id @default(cuid())
  email           String    @unique
  username        String    @unique
  firstName       String
  lastName        String
  role            String    // 'Admin', 'Manager', 'User'
  avatar          String?
  passwordHash    String
  salt            String
  isEmailVerified Boolean   @default(false)
  createdAt       DateTime  @default(now())
  lastLoginAt     DateTime?
}
```

#### Item (Article)
```prisma
model Item {
  id                 String    @id @default(cuid())
  name               String
  category           String
  dateAdded          DateTime  @default(now())
  quantity           Int
  status             String    // 'In Stock', 'Low Stock', 'Out of Stock'
  expectedReturnDate DateTime?
  movements          Movement[]
}
```

#### Movement (Mouvement)
```prisma
model Movement {
  movementId         String    @id @default(cuid())
  timestamp          DateTime  @default(now())
  type               String    // 'Entrée', 'Sortie'
  itemId             String
  itemName           String
  handledBy          String
  quantity           Int
  expectedReturnDate DateTime?
  actualReturnDate   DateTime?
  status             String
}
```

#### Invitation
```prisma
model Invitation {
  id        String   @id @default(cuid())
  email     String   @unique
  role      String
  token     String   @unique
  expiresAt DateTime
  createdBy String
  used      Boolean  @default(false)
}
```

---

## 🌐 Déploiement

### Déploiement sur Vercel (Recommandé)

1. **Créer un compte Vercel** sur [vercel.com](https://vercel.com)

2. **Connecter votre repository GitHub**

3. **Configurer les variables d'environnement** dans Vercel :
   - `DATABASE_URL`
   - `JWT_SECRET`
   - `EMAIL_SERVER_*` (si emails activés)

4. **Déployer** :
```bash
vercel --prod
```

### Déploiement manuel

```bash
# Build de production
npm run build

# Démarrer le serveur
npm run start
```

### Configuration PostgreSQL en production

Pour une base de données PostgreSQL hébergée, vous pouvez utiliser :
- **Vercel Postgres**
- **Supabase**
- **Railway**
- **Neon**
- **AWS RDS**

---

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. **Fork** le projet
2. Créez votre **branche de fonctionnalité** (`git checkout -b feature/NouvelleFonctionnalite`)
3. **Committez** vos changements (`git commit -m 'Ajout d'une nouvelle fonctionnalité'`)
4. **Push** vers la branche (`git push origin feature/NouvelleFonctionnalite`)
5. Ouvrez une **Pull Request**

### Standards de code

- Utiliser **TypeScript** pour tout nouveau code
- Suivre les conventions **ESLint** du projet
- Écrire des **commentaires clairs** en français
- Tester les fonctionnalités avant de soumettre

---

## 👨‍💻 Auteur

**Iliass KAOUACHI** - [@Ilykao171](https://github.com/Ilykao171)

Projet développé dans le cadre d'un stage chez **Stellantis**

---

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

MIT License - Copyright (c) 2025 Iliass KAOUACHI (@Ilykao171)

Permission est accordée, gratuitement, à toute personne obtenant une copie de ce logiciel et des fichiers de documentation associés, de traiter le logiciel sans restriction, y compris sans limitation les droits d'utiliser, copier, modifier, fusionner, publier, distribuer, sous-licencier et/ou vendre des copies du logiciel.

---

## 🙏 Remerciements

- **Stellantis** pour l'opportunité de développer ce projet
- La communauté **Next.js** et **React**
- Tous les mainteneurs des bibliothèques open source utilisées

---

## 📞 Support

Pour toute question ou problème :
- Ouvrir une **issue** sur GitHub

---

## 🗺️ Roadmap

### Version 1.1 (À venir)
- [ ] Notifications push
- [ ] Scan de codes-barres/QR codes
- [ ] Application mobile native
- [ ] Intégration avec systèmes ERP

### Version 1.2
- [ ] Gestion multi-sites
- [ ] Prévisions de stock par IA
- [ ] API publique documentée
- [ ] Webhooks pour intégrations tierces

---

**Dernière mise à jour :** 31 Octobre 2025
