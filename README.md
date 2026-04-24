# LokalPay Congo — Projet CG-02 | MIABE Hackathon 2026

**Inclusion financière & Réputation**  
*Young-Tech-CG*  

---

##  Résumé

**LokalPay Congo** est une application blockchain qui permet aux **commerçants informels des marchés de Brazzaville** (marché Total, marché Moungali, marché du Plateau) de construire un **historique de transactions vérifiable** et un **score de réputation** afin d’accéder au crédit et à de meilleures opportunités commerciales.

Les institutions de microfinance et les fournisseurs peuvent **consulter ce profil de réputation public** (avec l’accord du commerçant) pour prendre des décisions éclairées.

---

##  Contexte & Problème

- **Plus de 60 %** de l’emploi urbain à Brazzaville est informel.  
- **Moins de 15 %** des commerçants des marchés possèdent un compte bancaire.  
- **90 %** des demandes de microcrédit sont refusées faute d’historique de crédit.  
- Pourtant **45 %** des adultes congolais utilisent déjà le mobile money.

Un commerçant peut être honnête et régulier depuis 10 ans, mais il n’a **aucune preuve** de son sérieux. La solution doit **transformer son activité économique informelle en preuve vérifiable**.

---

## Ce que fait LokalPay

-  **Enregistrement des transactions** (ventes, achats, paiements entre commerçants) depuis un simple téléphone mobile.  
-  **Historique immuable** inscrit sur une blockchain publique (Celo), impossible à falsifier.  
-  **Score de réputation** calculé automatiquement à partir des transactions réelles (volume, régularité, diversité des partenaires, évaluations mutuelles).  
-  **Profil de réputation public** consultable par les microfinances et les fournisseurs via QR code.  
-  **Système de notation mutuelle** entre commerçants partenaires pour renforcer la confiance.

---

##  Utilisateurs finaux

- **Commerçants informels** des marchés de Brazzaville et Pointe-Noire  
- **Institutions de microfinance** cherchant des emprunteurs avec historique vérifiable  
- **Fournisseurs et grossistes** évaluant la solvabilité de nouveaux détaillants  
- **Associations de commerçants** des marchés congolais  

---

##  Pourquoi la blockchain ?

La blockchain choisie est **Celo**, une couche 1 optimisée pour l’inclusion financière mobile :

- **Immuabilité** : chaque transaction est gravée définitivement, aucune falsification possible.  
- **Transparence** : le calcul du score est public et vérifiable mathématiquement.  
- **Décentralisation** : pas de tiers de confiance central, l’historique survit à l’application.  
- **Accessible** : fonctionne avec un simple smartphone, adresses liées aux numéros de téléphone (compatible mobile money).  
- **Frais ultra-faibles** adaptés aux microtransactions des marchés.

---

##  Architecture (version MVP)

```
Application mobile commerçant (React Native / Flutter)
        │
        ▼
  Relayer Celo / Wallet Connect ──► Blockchain Celo (testnet/mainnet)
        │
        ▼
  Backend d'indexation (optionnel) ──► Interface microfinance (Web)
        │
        ▼
  Smart Contracts : Registre d'identité, Score de réputation, Évaluations
```

---

##  Livrables du Hackathon

1. **Document PDF de problématique** (données chiffrées)  
2. **Maquettes visuelles** (Figma)  
3. **Site web vitrine** (HTML/CSS/JS – voir section « Démo »)  
4. **Document blockchain** (plan technique, choix Celo, données on-chain, calcul du score)  
5. **Vidéo de présentation** (3-5 min)  
6. **MVP complet** (application commerçant + interface microfinance)  
7. **Documentation & Pitch de 10 minutes**

---

##  Démo

- **Site vitrine** : [Lien vers le site vitrine](https://lokalpay-congo.vercel.app) *(à remplacer par ton URL une fois hébergé)*  
- **Application mobile** (prototype) : bientôt disponible  

Pour voir le site en local :
```bash
git clone https://github.com/ton-compte/lokalpay-congo.git
cd lokalpay-congo
# Ouvrir index.html dans le navigateur
```

---

##  Données d'exemple

| Commerçant | Marché | Score | Transactions |
|------------|--------|-------|--------------|
| Maman Pauline | Marché Total, Brazzaville | 780/1000 | 234 |
| Papa Jean | Marché Moungali | 620/1000 | 112 |

---

##  Impact attendu

- **Inclusion financière** : des dizaines de milliers de commerçants sortent de l’invisibilité.  
- **Accès au crédit** : le score de réputation remplace le scoring bancaire inexistant.  
- **Formalisation progressive** : l’historique blockchain ouvre la voie à des services d’assurance et d’épargne.  

*Des plateformes similaires au Kenya ont augmenté l’accès au crédit de 35 %.*

---

##  Technologies utilisées

- **Blockchain** : Celo (smart contracts en Solidity)  
- **Frontend** : HTML5, CSS3, JavaScript (site vitrine) / React Native (application mobile)  
- **Backend** : Node.js (indexation), IPFS (stockage de documents)  
- **Design** : Figma  

---

##  Équipe

**Darollo Technologies Corporation** – Projet réalisé dans le cadre du **MIABE Hackathon 2026**, édition Congo Brazzaville.

---

## Licence

MIT – Libre d’utilisation pour des fins non commerciales et éducatives.  
Toute utilisation commerciale doit être validée par les auteurs.