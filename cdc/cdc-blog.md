# Cahier des charges du blog

## Contexte

### Présentation
Un responsable de formation d'une école de développement web souhaite mettre un blog à disposition de ses élèves.

### Objectif
Mettre à disposition un blog de développeurs souhaitant partager leur parcours lors de la formation O'clock... en réalité il s'agit d'un projet de blog standard à but pédagogique :nerd_face: ...

### Budget
A partir de 2000€ HT (soit 5 jours), réparti en :

- Gestion de projet (étude, cahier des charges, wireframes, suivi du dossier).
- Création des maquettes graphiques.
- Intégration HTML/CSS.
- Développement du blog.
- Tests et mise en ligne.

### Délai
Deux semaines à compter de la validation du devis (accompagné d'un acompte de 30%).

## Spécifications fonctionnelles

### Apparence
 - Ambiance lié à l'espace (_"cosmos"_)
 - Site responsive
 
### Contenus
  - des articles
  - des auteurs
  - des catégories (front, back, collaboration, vie du développeur)
 
Les contenus seraient créés à terme via une interface d'administration (à mettre en option, dans un premier temps nous vous fournirons les contenus).

### Interactions services
  - Liens et/ou partages vers les réseaux sociaux.
  - Champ de recherche

### Langue
Le site seré rédigé et présenté en français

### Arborescence
   - Accueil (liste d'articles)
   - Page catégorie (articles filtrés par catégorie)
      - Teamback
      - Teamfront
      - Collaboration
      - MaVieDeDev
   - Page auteur (articles filtrés par auteur)
      - [liste des auteurs]
   - Page article (détail d'un article)
   - (Contact)
   - (Mentions légales)
   - (Admin)

### Navigation
  - Un menu principal vers les catégories et l'accueil
    - En responsive, on affiche plutôt un menu burger dans lequel se trouvent les liens
  - Le titre d'un article dans une liste permet d'en afficher les détails
  - Dans la liste d'article ou sur la page d'un article, cliquer sur le nom d'une catégorie m'amène sur la page de cette catégorie
  - Un menu sur le côté avec un lien vers les pages des catégories et des auteurs
  - Un menu secondaire (dans le footer ou ailleurs) pour lier vers admin, contact, mentions légales

### Templates

### Layout global
   - Un menu avec :
      - Titre/logo.
      - Liens vers les catégories.
  - Une image d'en-tête avec titre + slogan (baseline).
  - "Sidebar" à droite qui regroupe :
      - Champ de recherche.
      - Liste des catégories.
      - Liste des auteurs.
  - Pied de page :
      - Liens vers les réseaux sociaux.
      - Liens vers admin, contact, mentions légales.

### Liste d'articles
  - Un article :
      - Un titre (cliquable)
      - Un résumé
      - Date
      - Auteur
      - Catégorie
  - Pagination "Précedente" et "Suivante"

### Contraintes techniques
  - Site responsive
  - Compatibilité dernières versions des navigateurs (Chrome, Firefox, Internet Explorer 11 et Edge)

## Spécifications techniques

### Architecture logicielle choisie

#### Côté front
  - HTML5 : le code respectera une sémantique correcte.
  - CSS : nous utiiserons CSS dans sa version 2 ou 3, pour rester compatible avec Internet Explorer 11. L'utilisation d'un framework pour le responsive est envisagé.
  - Javascript : sera utilisé si besoin, avec parcimonie.

#### Côté back
  - PHP : PHP7 sera utilisé. La classe PDO permettra d'accéder aux données MySQL
  - MySQL : permettra de stocker nos données

### Description des données
  - Articles
    - Titre
    - Résumé
    - Date du publication
    - Nombre du vues
    - Auteur de l'article
    - Catégorie à laquelle appartient l'article
  - Auteurs
    - Nom
    - Prénom
    - Image de profil
  - Catégories
    - Intitulé
