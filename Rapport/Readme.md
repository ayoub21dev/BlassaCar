---
marp: true
theme: default
_class: lead
_paginate: false
paginate: true
backgroundColor: #ffffff
style: |
  section {
    font-size: 22px;
    color: #333;
    line-height: 1.6;
    padding: 60px 80px;
  }
  footer { width: 100%; text-align: right; font-size: 14px; color: #888; }
  .logo-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: absolute;
    top: 40px;   
    left: 60px;
    right: 60px;
  }
  .logo-header img { height: 140px; margin: 0; margin-left:10px; margin-right:10px }
  h1 { color: #088dc7; font-size: 2.8em; margin-top: 100px; text-align: left; }
  h2 { color: #088dc7; font-size: 2em; border-bottom: 2px solid #088dc7; margin-bottom: 40px;}
  h3 { text-align: left; color: #444; margin-top: 0; }

  .sommaire-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin-top: 20px;
  }
  .sommaire-item {
    display: flex;
    align-items: center;
    background: #f4faff;
    border-radius: 12px;
    padding: 15px 20px;
    border-left: 5px solid #088dc7;
  }
  .sommaire-num {
    background: #088dc7; color: white; width: 35px; height: 35px;
    display: flex; justify-content: center; align-items: center;
    border-radius: 50%; font-weight: bold; margin-right: 15px; flex-shrink: 0;
  }

  .img-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 100%;
  }
  .img-methodo {
    width: 90%;
    height: auto;
    max-height: 700px;
    object-fit: contain;
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
  }
  .img-sprint {
    width: auto;
    height: auto;
    max-height: 500px;
    max-width: 95%;
    object-fit: contain;
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
  }

  .dt-card {
    background: #f0f7fa;
    padding: 30px;
    border-radius: 10px;
    border-top: 6px solid #088dc7;
    text-align: left;
    margin-top: 20px;
    width: 100%;
  }

  .tech-container {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 20px;
  }
  .badge-simple {
    padding: 8px 18px;
    border-radius: 6px;
    font-weight: 600;
    background-color: #545353ff;
    color: #ffffff !important;
    font-size: 0.85em;
    border: 1px solid #222;
  }
  .maquette-grid {
    display: flex;
    gap: 15px;
    justify-content: center;
    align-items: flex-start;
    min-height: 400px;
  }
  section.class-diagram-slide {
    padding: 35px 45px;
  }
  section.class-diagram-slide h2 {
    margin-bottom: 12px;
  }
  .class-diagram-container {
    justify-content: flex-start;
    gap: 8px;
  }
  .class-diagram-img {
    width: auto !important;
    max-width: 100%;
    max-height: 72vh !important;
    object-fit: contain;
  }
---

<div class="logo-header">
  <img src="images/ofppt-logo.png" alt="Logo Left">
  <img src="images/logo-solicode.png" alt="Logo Right">
</div>

# **Projet de Fin de Formation**

### BlassaCar — Plateforme de covoiturage entre les villes du Maroc

**Réalisé par :** <span class="highlight">Ayoub Jalyta</span>  
**Encadré par :** <span class="highlight">M. ESSARRAJ Fouad</span>  
**Filière :** Développement Mobile et Web

---

## Sommaire

<div class="sommaire-grid">
  <div class="sommaire-item"><div class="sommaire-num">1</div><div class="sommaire-text">Contexte du projet</div></div>
  <div class="sommaire-item"><div class="sommaire-num">2</div><div class="sommaire-text">Méthodologie de travail</div></div>
  <div class="sommaire-item"><div class="sommaire-num">3</div><div class="sommaire-text">Branche Fonctionnelle</div></div>
  <div class="sommaire-item"><div class="sommaire-num">4</div><div class="sommaire-text">Branche Technique</div></div>
  <div class="sommaire-item"><div class="sommaire-num">5</div><div class="sommaire-text">Conception</div></div>
  <div class="sommaire-item"><div class="sommaire-num">6</div><div class="sommaire-text">Démonstration</div></div>
  <div class="sommaire-item"><div class="sommaire-num">7</div><div class="sommaire-text">Conclusion</div></div>
</div>

---

## 1. Contexte du projet

<div class="img-container">
  <img src="images/Context.png" class="img-sprint" alt="Contexte du projet">
</div>

---

## 2. Méthodologie : Design Thinking

<div class="img-container">
  <img src="images/designThinking.png" class="img-methodo" alt="Design Thinking">
</div>

---

## Méthodologie : Scrum (Agile)

<div class="img-container">
  <img src="images/scrum.jpg" class="img-methodo" alt="Scrum">
</div>

---

## Méthodologie : Processus 2TUP

<div class="img-container">
  <img src="images/2TUP.png" class="img-methodo" alt="2TUP">
</div>

---

## 3. Branche Fonctionnelle : Design Thinking

### 1. EMPATHIE

<div class="img-container">
  <div class="dt-card" style="border-top-color: #f39c12;">
    <h4>Comprendre l'utilisateur</h4>
    <blockquote style="font-style: italic; background: white; padding: 15px; border-radius: 8px;">
      <p>- <strong>Mohamed (Conducteur, 28 ans)</strong> passe 60% de son temps à gérer des messages WhatsApp pour trouver des passagers. Il veut partager ses frais de carburant mais n'a aucun outil fiable pour organiser ses trajets.</p>
      <p>- <strong>Fatima (Voyageuse, 22 ans)</strong> cherche des trajets bon marché entre les villes mais ne trouve que des groupes Facebook désorganisés, sans vérification des conducteurs ni garantie de sécurité.</p>
      <p>- <strong>Karim (Administrateur, 30 ans)</strong> doit modérer manuellement les profils et les trajets sans aucun tableau de bord centralisé, ce qui le rend incapable de détecter les fraudes en temps réel.</p>
    </blockquote>
  </div>
</div>

---

## Branche Fonctionnelle : Design Thinking

### 2. DÉFINITION

<div class="img-container">
  <div class="dt-card" style="border-top-color: #f39c12;">
    <h4>Cadrage du problème</h4>
    <blockquote style="font-style: italic; background: white; padding: 15px; border-radius: 8px;">
      <p>- Comment pourrions-nous <strong>centraliser</strong> la publication et la recherche de trajets en une seule plateforme, sans passer par Facebook ou WhatsApp ?</p>
      <p>- Comment pourrions-nous <strong>instaurer la confiance</strong> entre conducteurs et voyageurs inconnus grâce à la vérification de profil (CIN + téléphone) et un système de notation ?</p>
      <p>- Comment pourrions-nous donner à l'administrateur un <strong>tableau de bord proactif</strong> avec alertes en temps réel pour modérer la plateforme efficacement ?</p>
    </blockquote>
  </div>
</div>

---

## Branche Fonctionnelle : Design Thinking

### 3. IDÉATION

<div class="img-container">
  <div class="dt-card" style="border-top-color: #f39c12;">
    <h4>Solutions retenues</h4>
    <p>• Interface de <strong>publication de trajet en 2 minutes</strong> pour le conducteur (from, to, date, seats, price).</p>
    <p>• <strong>Système de vérification</strong> CIN + téléphone pour instaurer la confiance dès l'inscription.</p>
    <p>• <strong>Notifications WhatsApp</strong> automatiques à chaque confirmation de réservation.</p>
    <p>• <strong>Dashboard Admin</strong> avec KPIs en temps réel : trajets actifs, signalements, statistiques.</p>
    <p>• Modèle de démarrage <strong>gratuit</strong> pour construire la base d'utilisateurs, puis commission de 10% par réservation.</p>
  </div>
</div>

---

## Branche Fonctionnelle : Cas d'utilisation

<div style="text-align: center; width: 115%; margin-left: -7.5%; margin-top: -20px;">
  <img src="images/useCaseGlobalee.png" style="width: 100%; height: auto; max-height: 80vh; object-fit: contain; border-radius: 12px; box-shadow: 0 12px 40px rgba(0,0,0,0.2);" alt="Use Case Global">
</div>

---

## Branche Fonctionnelle : Sprint 1 (MVP)

<div class="img-container" style="height: auto;">
  <img src="images/sprint1.png" class="img-sprint" alt="Sprint 1">
</div>

---

## Branche Fonctionnelle : Sprint 2

<div class="img-container" style="height: auto;">
  <img src="images/sprint2.png" class="img-sprint" alt="Sprint 2">
</div>

---

## Branche Fonctionnelle : Maquettes - Landing Page

<div class="img-container">
  <img src="images/HomePage.png" class="img-methodo" style="height: 500px; width: auto;" alt="Public Landing">
  <p style="font-size: 0.9rem; color: #666; margin-top: 10px;">Page d'accueil de la plateforme</p>
</div>

---

## Branche Fonctionnelle : Maquettes - Admin

<div class="img-container">
  <img src="images/AdminDashbord.png" class="img-methodo" style="height: 500px; width: auto;" alt="Interface Administration">
  <p style="font-size: 0.9rem; color: #666; margin-top: 10px;">Tableau de bord de l'administrateur</p>
</div>

---

## Branche Fonctionnelle : Maquettes - Chauffeur

<div class="img-container">
  <img src="images/DriverDashbord.png" class="img-methodo" style="height: 500px; width: auto;" alt="Interface Chauffeur">
  <p style="font-size: 0.9rem; color: #666; margin-top: 10px;">Tableau de bord du conducteur</p>
</div>

---

## Branche Fonctionnelle : Maquettes - Voyageur

<div class="img-container">
  <img src="images/TravelrDashobrd.png" class="img-methodo" style="height: 500px; width: auto;" alt="Interface Voyageur">
  <p style="font-size: 0.9rem; color: #666; margin-top: 10px;">Tableau de bord du voyageur</p>
</div>

---

## 4. Branche Technique : Tech Stack

<div class="sommaire-grid">
  <div class="dt-card" style="margin-top:0;">
    <h4>Les technologies à utiliser</h4>
    <ul>
      <li><strong>Base de données:</strong> MySQL </li>
      <li><strong>Framework:</strong> Laravel 12</li>
      <li><strong>Architecture:</strong> N-Tiers</li>
      <strong>Controller:</strong> Requêtes HTTP
      <strong>Service:</strong> Logique métier
      <strong>Model:</strong> Base de données
      <li><strong>Architecture:</strong> MVC</li>
      <li><strong> Blade :</strong>Templates réutilisables (components, layouts).</li>
    </ul>
  </div>
  <div class="dt-card" style="margin-top:0; border-top-color: #27ae60;">
    <ul>
      <li><strong>Alpine.js :</strong> Librairie JavaScript pour les interactions dynamiques.</li>
      <li><strong>Spatie :</strong> Librairie pour la gestion des permissions et rôles.</li>
      <li><strong>Vite :</strong> Outil de build rapide.</li>
      <li><strong>Lucide :</strong> Librairie d'icônes.</li>
      <li><strong>Tailwind CSS :</strong> Développement rapide, responsive.</li>
    </ul>
  </div>
</div>

---

<!-- _class: class-diagram-slide -->
## 5. Conception : Diagrammes UML

<div class="img-container class-diagram-container">
   <h3>Modélisation des données (MLD)</h3>
  <img src="images/digramedeClass.png" class="img-methodo class-diagram-img" alt="Diagramme de classe">
</div>

---

## 6. Démonstration : Environnement & Outils

<div class="sommaire-grid">
  <div class="dt-card" style="margin-top:0;">
    <h4>Environnement de Développement</h4>
    <ul>
      <li><strong>IDE :</strong> VS Code & Antigravity </li>
      <li><strong>Monitoring DB :</strong> Workbench Sql</li>
    </ul>
  </div>
  <div class="dt-card" style="margin-top:0; border-top-color: #27ae60;">
    <h4>Gestion & Déploiement</h4>
    <ul>
      <li><strong>Modelisation UML :</strong> Mermaid/PlantUML</li>
      <li><strong>Gestion de version :</strong> Git (GitHub)</li>
      <li><strong>Navigateur :</strong> Chrome DevTools</li>
    </ul>
  </div>
</div>

<br>

---

## 7. Conclusion

- **Objectifs atteints** : Plateforme BlassaCar fonctionnelle et responsive.
- **Compétences** : Maîtrise du cycle Agile, Design Thinking et de la stack Full-stack Laravel.
- **Perspectives** : Intégration d'un module de paiement en ligne (CMI) et d'une application mobile.

<br>

### Merci pour votre attention !
