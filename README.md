# 🏥 SantéZig — Plateforme IA de Pré-enregistrement, Triage et Gestion des Flux de Santé

**Projet Académique — L3 Ingénierie Informatique (2025–2026)**  
**Université Assane Seck de Ziguinchor (UASZ)** — *Cours : Innovations Technologiques en IA*  
**Groupe n° 8** : Thierno Ibrahima Ba, Mouhamed Ngom, Sokhna Diarra Bousso Fall, Arona Ndaw, Mame Faty Diop

---

## 🎯 1. Problématique & Objectif
Les structures sanitaires de la région de Ziguinchor font face à un engorgement quotidien dû à l'afflux de consultations de routine et à l'absence de système de triage structuré à l'accueil.

**SantéZig** répond à ce défi en proposant :
* **Le pré-enregistrement intelligent** (à distance sur smartphone ou sur borne agent d'accueil).
* **L'identification sécurisée par Carte Nationale d'Identité (CNI / NIN)** et suivi des maladies chroniques.
* **L'accessibilité totale (Multilingue & Vocale)** : interface traduite en **Français, Wolof, Diola (Joola), Poular (Pulaar) et Anglais**, accompagnée d'une **dictée vocale automatique** et d'une **note vocale audio** pour les patients ne sachant ni lire ni écrire.
* **Le triage assisté par IA** classant automatiquement les patients en 3 niveaux (**1 : URGENT**, **2 : PRIORITAIRE**, **3 : ROUTINE**) avec détection des drapeaux rouges cliniques.
* **Le contrôle humain obligatoire (*Human-in-the-loop*)** : validation médicale, réévaluation en urgence et fiche d'observation clinique.
* **Le pilotage régional** : statistiques en temps réel, prévision des heures de pointe, export CSV et rapport officiel imprimable.

---

## 📁 2. Organisation du dépôt GitHub (`santezig-platform`)
```text
santezig-platform/
├── index.html          # Prototype complet autonome (Patient, Médecin, Stats & Rapports)
├── backend/
│   ├── app.py          # API REST Flask + Base de données SQLite
│   ├── model_triage.py # Modèle Machine Learning (RandomForest + règles cliniques)
│   └── requirements.txt
└── README.md           # Documentation & Guide de déploiement