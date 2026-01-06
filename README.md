#  Mastering HashiCorp Vault

<div align="center">

![Vault Logo](https://img.shields.io/badge/HashiCorp-Vault-7B42BC?style=for-the-badge&logo=vault&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-Documentation-008080?style=for-the-badge&logo=latex&logoColor=white)
![License](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey?style=for-the-badge)

**Guide technique complet pour la gestion sécurisée des secrets avec HashiCorp Vault**

[📖 Documentation](#documentation) • [🚀 Démarrage](#démarrage-rapide) • [💡 Fonctionnalités](#fonctionnalités) • [🤝 Contribution](#contribution)

</div>

---

##  À propos

Cette documentation technique offre une exploration exhaustive de **HashiCorp Vault**, la solution de référence pour la gestion centralisée et sécurisée des secrets en environnement DevOps et cloud-native. 

Conçue pour les professionnels de la cybersécurité, ingénieurs DevSecOps et architectes cloud, cette ressource combine :
-  Fondamentaux théoriques
-  Tutoriels pratiques détaillés  
-  Études de cas réels
-  Bonnes pratiques de production

##  Objectifs

-  Comprendre l'architecture et les composants de Vault
-  Maîtriser la configuration et le durcissement sécuritaire
-  Implémenter des politiques d'accès granulaires
-  Intégrer Vault dans les pipelines CI/CD
-  Gérer la haute disponibilité et le disaster recovery
-  Assurer la conformité et l'audit

##  Documentation

### Structure du document

Le guide est organisé en 17 chapitres couvrant :

1. **Introduction à HashiCorp Vault** - Concepts fondamentaux et architecture
2. **Installation et Configuration** - Déploiement sur Linux, Docker et Kubernetes
3. **Premiers Pas** - Interface CLI et Web UI
4. **Secrets Engines** - KV, Database, AWS, Transit, PKI
5. **Méthodes d'Authentification** - Token, UserPass, AppRole, Kubernetes
6. **Policies et Contrôle d'Accès** - ACL et gestion des permissions
7. **Configuration Production** - Setup HA et sécurisation
8. **Projet Pratique** - Application Flask intégrée avec Vault
9. **Haute Disponibilité** - Clustering et réplication
10. **Intégration Kubernetes** - Vault Agent Injector
11. **Monitoring et Troubleshooting** - Prometheus, Grafana
12. **Sécurité Avancée** - Rotation, révocation, response wrapping
13. **Bonnes Pratiques** - Architecture recommandée et checklist
14. **Cas d'Usage Avancés** - PKI, SSH, TOTP
15. **Conformité et Audit** - Logging et rapports
16. **Commandes Utiles** - Référence CLI
17. **Guide de Dépannage** - Solutions aux problèmes courants

### Compilation du document

```bash
# Cloner le dépôt
git clone https://github.com/maryeeem/mastering-vault-hashicorp.git
cd mastering-vault-hashicorp

# Compiler le document LaTeX
pdflatex main.tex
pdflatex main.tex  # Seconde compilation pour les références

# Ou utiliser latexmk
latexmk -pdf main.tex
```

## Démarrage rapide

### Prérequis

- **LaTeX Distribution** : TeX Live (Linux), MacTeX (macOS), MiKTeX (Windows)
- **Packages requis** : 
  - babel, graphicx, hyperref, xcolor
  - listings, float, geometry
  - fancyhdr, tcolorbox, enumitem
  - tikz, fontawesome5

### Installation rapide

```bash
# Ubuntu/Debian
sudo apt-get install texlive-full texlive-lang-french

# macOS avec Homebrew
brew install --cask mactex

# Vérifier l'installation
pdflatex --version
```

##  Fonctionnalités

### 🔹 Contenu technique

- **Architecture détaillée** avec diagrammes explicatifs
- **Exemples de code** annotés et testés
- **Configurations prêtes à l'emploi** pour Docker Compose
- **Scripts d'automatisation** Python et Bash
- **Intégration CI/CD** avec Jenkins, GitLab CI
- **Monitoring avancé** avec Prometheus/Grafana

### 🔹 Projet pratique inclus

Application Flask démontrant :
- Authentification AppRole
- Génération de credentials dynamiques PostgreSQL
- Chiffrement/déchiffrement avec Transit Engine
- Gestion du cycle de vie des secrets

**🔗 Code source** : [myapp-vault](https://github.com/maryeeem/myapp-vault.git)

### 🔹 Ressources visuelles

- 50+ captures d'écran détaillées
- Schémas d'architecture professionnels
- Diagrammes de flux explicatifs
- Mise en forme professionnelle avec couleurs thématiques

##  Structure du projet

```
mastering-vault-hashicorp/
├── main.tex                    # Document principal
├── vault.png                   # Logo Vault
├── images/                     # Screenshots et diagrammes
│   ├── vault_architecture_overview.png
│   ├── vault_kv_put_output.png
│   ├── vault_cluster_status.png
│   └── ...
├── scripts/                    # Scripts d'automatisation
│   ├── setup-vault.sh
│   ├── configure-db-engine.sh
│   └── compliance-report.py
├── configs/                    # Fichiers de configuration
│   ├── vault.hcl
│   ├── docker-compose.yml
│   └── policies/
├── README.md
└── LICENSE
```

## 🛠️ Technologies couvertes

- **HashiCorp Vault** 1.15+
- **Docker & Docker Compose**
- **Kubernetes** (Helm, PV/PVC)
- **PostgreSQL** (Dynamic Credentials)
- **Python** (hvac library)
- **Flask** (Application web)
- **Prometheus & Grafana** (Monitoring)
- **AWS KMS** (Auto-Unseal)

## 📚 Ressources complémentaires

-  [Documentation officielle Vault](https://developer.hashicorp.com/vault)
-  [HashiCorp Learn Platform](https://learn.hashicorp.com/vault)
-  [Community Forum](https://discuss.hashicorp.com/c/vault)
-  [Vault sur GitHub](https://github.com/hashicorp/vault)



##  Licence

Ce projet est sous licence **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International** (CC BY-NC-SA 4.0).

Vous êtes libre de :
-  **Partager** — copier et redistribuer le matériel
-  **Adapter** — remixer, transformer et créer à partir du matériel

Selon les conditions suivantes :
-  **Attribution** — Vous devez créditer l'œuvre
- **Pas d'utilisation commerciale** — Vous ne pouvez pas utiliser cette œuvre à des fins commerciales
-  **Partage dans les mêmes conditions** — Si vous modifiez l'œuvre, vous devez distribuer votre contribution sous la même licence

Voir le fichier [LICENSE](LICENSE) pour plus de détails.

##  Auteure

**Maryem Cherif**  
 Network Security Engineer | Passionnée de Cybersécurité

- 🌐 GitHub: https://github.com/maryeeem
- 📧 Email: cherif.maryem24@gmail.com 
- 💼 LinkedIn: www.linkedin.com/in/cherif-maryem 

---

## 🌟 Remerciements

Un grand merci à :
- La communauté **HashiCorp** pour l'excellente documentation
- Les contributeurs **Open Source** qui inspirent ce travail
- Les **reviewers** qui ont aidé à améliorer ce document

---


<div align="center">

**⭐ Si ce projet vous a été utile, n'hésitez pas à lui donner une étoile !**

*« La sécurité n'est pas une destination, c'est un voyage continu. »*

</div>
