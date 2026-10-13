# intelligent-photovoltaic-cleaning-platform
Plateforme web intelligente de gestion de centrales photovoltaïques et d'optimisation des opérations de nettoyage, basée sur la vision par ordinateur (YOLOv8).

## Fonctionnalités
- Tableau de bord et suivi des centrales photovoltaïques
- Carte interactive des centrales
- Analyse d'images par YOLOv8 (détection de salissures sur les panneaux)
- Alertes, historique des analyses et des nettoyages
- Priorisation des interventions de nettoyage
- Rapports et gestion des comptes utilisateurs

## Architecture
- `ai-model/` : entraînement et analyse du modèle YOLOv8
- `api.py` : API Python d'inférence
- `backend/` : API Node.js (authentification, centrales, analyses, alertes, nettoyage)
- `frontend/` : interface React (Vite)

## Modèle YOLOv8
Les poids du modèle sont trop lourds pour GitHub : [télécharger le modèle](https://drive.google.com/drive/u/0/folders/1zQ73gaG17MzdioJitc-yOEzXMDAoUIMC)

## Installation
### Backend
    cd backend
    npm install
    npm start

### Frontend
    cd frontend
    npm install
    npm run dev

### API d'inférence
    pip install ultralytics flask
    python api.py

## Auteurs
- Yassine Haddar
- Ahmed Gaabi

Projet réalisé dans le cadre du PFA, ENET'Com Sfax.