# Ingénieur cybersécurité 

> **Objectif** : assurer les missions de RSSI | Directeur cyber | Manager SOC.

---

## À propos

Passionné de cybersécurité, consultant SSI depuis 10/2025, dernièrement 3 ans de gestion de projets SSI.
Reprise d'études supérieures CYBER de 2021 à 2025 : L2, L3, M1, M2, et Ingénieur), auparavant test startup (devApk), sur un fond de 10 ans d'admin/tech sys/réseaux.  

**3 projets publiés** 
&nbsp;&nbsp;Réalisation d'une attaque de type supercharging (sur superchargeur de véhicule éléctrique) par modèle IA non supervisé avec apprentisage, appels LLM et traiement du RAG. [07/2025] 
&nbsp;&nbsp;Réalisation d'un système de détection de l'attaque d'overcharging qui permet d'alimenter un SIEM. [07/2025]
&nbsp;&nbsp;Réalisation d'un application mobile favorisant la sécurité des victimes et des intervenants ainsi qu'un gain de temps, lors d'interventions de secours sur véhicules automobiles européens. [04/2016]  
&nbsp;&nbsp;Ecriture d'un livre titré "Accouchement innopiné interhospitalier". [07/2008] 

*6 projets récents non publiés** 
&nbsp;&nbsp;Convergence d'annuaires AD en un environnmeent durci à l'état de l'art (09/2025).
&nbsp;&nbsp;Téléphonie unifiée (Teams/DECT fixe/mobile) (08/2024).
&nbsp;&nbsp;SD-WAN migrations de multiples BU (02/2024).
&nbsp;&nbsp;SAP ERP déploiement sur une BU 10M€ (01/2024).
&nbsp;&nbsp;Renouvellement infrastructure réseaux/systèmes d'une BU (12/2023).
&nbsp;&nbsp;Pilotage XDR ESET (09/2022-08/2024).

**230+ Challenges de sécurité résolus**, participation active au Bug Bounty.

** passif secouriste 1991-2020**





---

## Plan du dépôt « Portfolio‑SSI »

```
Portfolio/
├─ README.md                # Page d’accueil principale (intro + sommaire + liens)
├─ hard-skills              # Compétences techniques détaillées
├─ soft-skills              # Qualités humaines et management
├─ expérience               # Expériences professionnelles
├─ formation                # Diplômes, formations, certifs
├─ projets/                 # Démonstrations et labos
│  ├─ Projet 1 (lab OWASP)
│  ├─ ad-attack-defense/
│  ├─ network-threat-hunt/
│  └─ ...
├─ challenges de sécurité réalisés/
│  ├─ writeups/
│  └─ index.md
└─ assets/                  # images, schémas, captures
```

> Conseil : 1 **projet = 1 mini‑démo reproductible** (README clair, étapes, IOCs/indicateurs, captures). Gardez les données sensibles fictives.

---

## Projets SSI (sélection)

> Remplacez les exemples par vos réels projets. Gardez un format constant : **problème → approche → résultat → reproductibilité**.

### 1) **Web OWASP Lab — from Recon to RCE**

* **Stack** : Nmap, dirsearch, Burp, ffuf, Python (exploits), Docker lab
* **Résumé** : Cartographie, IDOR & XSS → escalade → RCE en environnement containerisé.
* **Points clés** : méthodologie, PoC scripté, correctifs proposés.
* **Repo** : [`projets/web-owasp-lab`](./projets/web-owasp-lab) · 🎥 Demo GIF dans `assets/`

### 2) **Active Directory — Attack Paths & Detections**

* **Stack** : BloodHound/SharpHound, Mimikatz, Sigma/Rules → ELK
* **Résumé** : Construction d’un lab AD, chemins d’attaque, détections corrélées (Winlogbeat → ELK).
* **Repo** : [`projets/ad-attack-defense`](./projets/ad-attack-defense)

### 3) **Threat Hunting — Beaconing & DNS Tunneling**

* **Stack** : Zeek, Suricata, ELK, Python notebooks
* **Résumé** : Détection de beaconing, score DNS, visualisation et playbooks d’enquête.
* **Repo** : [`projets/network-threat-hunt`](./projets/network-threat-hunt)

> **Astuce** : Ajoutez des badges *Shields.io* pour la stack par projet (ex : `![Tool](https://img.shields.io/badge/Nmap-0078D4)`), et un GIF court de la démo.

---

## Root‑Me — Challenges & Write‑ups

### Statut & profils

* **Profil Root‑Me** : *(lien ici)*
* **Total résolus** : **XXX**
* Catégories fortes : Web‑Server, App‑Script, Forensic, Crypto

> **Mise en avant** : listez **5–10** challenges représentatifs avec *le skill appris* et *la technique clé*. Liez vos write‑ups.

| Catégorie  | Challenge                    | Compétence apprise | Technique clé           | Write‑up                                                                      |
| ---------- | ---------------------------- | ------------------ | ----------------------- | ----------------------------------------------------------------------------- |
| Web‑Server | XXE – Simple                 | XXE & exfiltration | Payload external entity | [/root-me/writeups/xxe-simple.md](./root-me/writeups/xxe-simple.md)           |
| App‑Script | NodeJS – Prototype Pollution | Audit JS runtime   | Gadget chain → RCE      | [/root-me/writeups/proto-pollution.md](./root-me/writeups/proto-pollution.md) |
| Forensic   | PCAP – Suspicious Beacon     | Network forensics  | JA3 + interval delta    | [/root-me/writeups/pcap-beacon.md](./root-me/writeups/pcap-beacon.md)         |
| Crypto     | RSA – Factorization          | Maths & tooling    | Fermat / Pollard Rho    | [/root-me/writeups/rsa-factor.md](./root-me/writeups/rsa-factor.md)           |

> **Bonne pratique** : Ne dévoilez **jamais** la solution brute si le challenge l’interdit. Rédigez plutôt une **cheminement d’analyse** + indices pédagogiques.

### Modèle de write‑up (copier‑coller)

```markdown
# [Root‑Me] <Catégorie> — <Nom du challenge>

## TL;DR
- **Objectif** : …
- **Vecteur** : …
- **Flag** : [redacted]

## 1. Reconnaissance / Analyse
- … captures `assets/` …

## 2. Exploitation / Résolution
- … commandes, payloads **expurgés** …

## 3. Leçons & Défenses
- … détection, règle Sigma, recommandations …
```

---
