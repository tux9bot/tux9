# RSSI | Directeur cybesécurité | Manager SOC | Architecte sécurité |

> **Objectif** : Présenter clairement mes projets SSI (offensif/défensif) et mes réussites Root‑Me. Ce modèle est prêt à copier‑coller dans votre README de profil ou dans un dépôt « Portfolio‑SSI ».

---

## À propos

Passionné de cybersécurité (2 ans d’admin système → reconversion SSI). 6 mois d’étude intensive : **100+ CTF résolus**, **10+ projets publiés**, participation active au Bug Bounty. Je cherche un poste **Junior Security Analyst / Pentester**.

**Stack clé** : OWASP Top 10 · Nmap · Wireshark · Burp Suite · Metasploit · Python · Bash · SQL · Linux/Kali · Windows/AD · ELK · Splunk · Docker/K8s (notions)

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

## 📦 Comment créer la page GitHub

### Option A — README de **profil** (recommandé)

1. Créez un dépôt **public** nommé **`ivan`** (exactement votre pseudo GitHub).
2. Ajoutez un fichier `README.md` et collez ce modèle.
3. Les visuels (`assets/`) s’affichent directement sur votre page de profil.

### Option B — Dépôt **Portfolio‑SSI**

1. Créez un repo `Portfolio-SSI`.
2. Copiez l’arborescence ci‑dessus et poussez vos projets dans `projets/`.
3. Mettez les write‑ups dans `root-me/writeups/`.

### Commandes Git (rappel rapide)

```bash
git init && git add .
git commit -m "feat: init portfolio ssi"
git branch -M main
git remote add origin git@github.com:ivan/Portfolio-SSI.git
git push -u origin main
```

---

## Blocs prêts‑à‑coller (badges & widgets)

**Badges stack**

```
![Linux](https://img.shields.io/badge/Linux-0B4?logo=linux)
![Kali](https://img.shields.io/badge/Kali-268BEE?logo=kalilinux)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python)
![Burp](https://img.shields.io/badge/Burp_Suite-FF7139)
![Nmap](https://img.shields.io/badge/Nmap-4F4F4F)
```

**Cartes de stats GitHub** (par anuraghazra)

```
![Stats](https://github-readme-stats.vercel.app/api?username=ivan&show_icons=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=ivan&layout=compact)
```

**Timeline d’activité**

```
![Streak](https://streak-stats.demolab.com?user=ivan)
```

---

## Checklist qualité

* [ ] README clair par projet (objectif, étapes, résultats, reproductible)
* [ ] Captures **anonymisées** & données **fictives**
* [ ] Licence (ex : `LICENSE` MIT) et `SECURITY.md` pour signaler une vulnérabilité
* [ ] `.gitignore` (ex : logs, secrets, dumps)
* [ ] Arborescence propre + badges + GIF de démo

---

## Contact & disponibilités

Ouvert aux opportunités **Pentest / Blue Team / AppSec**.
Écrivez‑moi : [tux@example.com](mailto:tux@example.com) 

---

### Annexes — Squelettes rapides

**`projets/<nom>/README.md`**

```markdown
# <Nom du projet>

## Objectif
…

## Environnement
- OS / versions
- Outils

## Étapes clés
1. …
2. …

## Résultats / IOCs
- …

## Limites & pistes
- …
```

**`root-me/index.md`**

```markdown
# Root‑Me — Sommaire

- Total : XXX
- Par catégorie : Web‑Server(X), App‑Script(Y), Forensic(Z), Crypto(W)

## Write‑ups
- [XXE – Simple](./writeups/xxe-simple.md)
- [Prototype Pollution](./writeups/proto-pollution.md)
- …
```

**`SECURITY.md` (modèle)**

```markdown
# Security Policy

## Reporting a Vulnerability
Please do not open public issues for security problems. Email <security@exemple.tld> with details and a repro.
```
