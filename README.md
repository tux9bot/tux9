# Ingénieur cybersécurité | 

> **Objectif** : mes projets SSI sont d'assurer les missions de RSSI | DSI | Directeur cybersécurité-Cyberdéfense | Manager SOC | Architecte sécurité expert | Chef de projets SSI.

---

## À propos

Passionné de cybersécurité (2 ans d’admin système → reconversion SSI). 6 mois d’étude intensive : **100+ CTF résolus**, **10+ projets publiés**, participation active au Bug Bounty. Je cherche un poste **Junior Security Analyst / Pentester**.

**Hard skillss** 
- comprendre la menace, manager des équipes opérationnelles et les conduire techniquement en situation de crise.
- conduire les équipes pendant build et run liés aux incidents de sécurité, capitaliser sur ses expériences.
- tenir le programme de sensibilisation cyber des collaborateurs (exercices de phishing et de gestion de crise)
- préparer les équipes aux certifications sur le volet sécurité du SI et cyber.
- analyser les risques ainsi que les impacts (par ex. sur les données personnelles), les menaces et les attaques.
- évaluer la maturité à gérer une crise d'origine cyber, organiser les exercice de gestion de crise
- auditer la sécurité d'un SI en constante évolution, appliquer les contre-mesures adaptées.
- deployer des architectures (fonctionnelles, de stockage, et de sauvegardes) sécurisées car durcies à l'état de l'art.
- assurer le durcissement système des terminaux (Windows et Linux) et de l'annuaire active directory (tiering, cycle d'amélioration continu SSI).
- mettre en œuvre un service de veille et de renseignement et d'intelligence de la menace (CTI).
- acquérir une expertise technique élevée en approfondissant mes connaissances.
- participer aux opérations de recherche fondamentale sur fond de SSI.

**Soft skills** 
- Esprit d’analyse, car je comprend rapidement une alerte ou un code suspect.
- Curiosité technique, car j'explore, teste, et cherche des vulnérabilités.
- Résilience et patience, j'ai l'habitude d'investigations rapides et longues.
Esprit critique → ne pas se fier à la première hypothèse.
Travail en équipe → SOC, pentest, projets collaboratifs
Pédagogie / vulgarisation → expliquer les risques aux non-techniques
Éthique → respecter la confidentialité, les chartes de test, la loi

**Outils**

---

## Plan du dépôt « Portfolio‑SSI »

```
Portfolio-SSI/
├─ README.md                # Page d’accueil (ce fichier)
├─ projets/
│  ├─ web-owasp-lab/        # Projet 1 (ex : lab OWASP)
│  ├─ ad-attack-defense/    # Projet 2 (ex : AD attack path)
│  ├─ network-threat-hunt/  # Projet 3 (ex : Hunt ELK)
│  └─ ...
├─ root-me/
│  ├─ writeups/             # Vos write-ups (un par challenge)
│  └─ index.md              # Sommaire + stats
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
