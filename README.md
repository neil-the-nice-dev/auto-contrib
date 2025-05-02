# 🌱 auto-contrib

:octocat: Ce projet génère automatiquement une contribution GitHub chaque jour grâce à GitHub Actions. Parfait pour garder une "pelouse verte" sur ton profil 🌿.

---

## 🚀 Comment l'utiliser

### 1. Créer un dépôt à partir de ce template
- Clique sur **"Use this template"** en haut à droite de la page.
- Ou suis la documentation officielle :  
  👉 [Créer un dépôt depuis un template](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template)

### 2. Ajouter les secrets nécessaires
Va dans ton dépôt → **Settings > Secrets and variables > Actions > New repository secret**  
Ajoute les deux secrets suivants :

| Nom du secret | Valeur attendue |
|---------------|------------------|
| `USER_EMAIL`  | Ton email GitHub (ex: `monmail@proton.me`) |
| `GH_PAT`      | Ton token GitHub personnel avec droits `repo` |

> 📌 [Créer un token GitHub personnel (classic)](https://github.com/settings/tokens/new)

---

### 3. Activer les permissions pour `git push`

GitHub bloque le `git push` dans les actions par défaut. Pour autoriser l'action à pousser du code :

- Va dans **Settings > Actions > General**
- Descends jusqu'à **"Workflow permissions"**
- Sélectionne **"Read and write permissions"**
- Clique sur **"Save"**

---

## 🔄 Ce que fait le workflow

- Le fichier `.github/workflows/fairy.yml` exécute tous les jours une action programmée.
- Il fait un **commit vide** à ton dépôt avec l'heure actuelle.
- Cela maintient une **activité quotidienne sur ton profil GitHub**, même si tu ne travailles pas ce jour-là.

---

## 🕒 Fréquence

L’action s’exécute automatiquement **tous les jours à 22h25 (heure de La Réunion, UTC+4, modifiable dnas les parametres)**.

---

## ❓ Besoin d’aide ?

Ouvre une issue ou contacte moi ✨
