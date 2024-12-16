# Créer un site web avec HTML5 et GitHub Pages

## 1. Préparer le projet localement

1. **Créer un dossier** sur votre ordinateur :  
  Exemple : `mon-site`.
  
2. **Créer un fichier `index.html`** :  
  Exemple de contenu minimal :
  
  ```html
  <!DOCTYPE html>
  <html lang="fr">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Mon Site</title>
  </head>
  <body>
      <h1>Bienvenue sur mon site</h1>
      <p>Ceci est mon premier site.</p>
  </body>
  </html>
  ```
  

---

## 2. Créer un dépôt GitHub

1. **Connectez-vous à GitHub** ou créez un compte : [GitHub](https://github.com).
2. **Créer un nouveau dépôt** :
  - Cliquez sur **"New repository"**.
  - Entrez un nom pour le dépôt, par exemple `mon-site`.
  - Sélectionnez **Public** (requis pour GitHub Pages).
  - **Ne cochez pas** "Add a README file".
  - Cliquez sur **Create repository**.

---

## 3. Lier le projet local à GitHub

1. **Ouvrez un terminal dans le dossier du projet** :
  
  ```bash
  cd mon-site
  ```
  
2. **Initialiser Git** :
  
  ```bash
  git init
  ```
  
3. **Ajouter et commit vos fichiers** :
  
  ```bash
  git add .
  git commit -m "Premier commit : ajout du site"
  ```
  
4. **Lier le dépôt local à GitHub** :
  - Copiez l'URL de votre dépôt (exemple : `https://github.com/<votre-utilisateur>/mon-site.git`).
  - Exécutez :
    
    ```bash
    git remote add origin https://github.com/<votre-utilisateur>/mon-site.git
    git branch -M main
    git push -u origin main
    ```
    

---

## 4. Activer GitHub Pages

1. **Accédez aux paramètres de votre dépôt** :
  - Cliquez sur l'onglet **Settings**.
2. **Configurer GitHub Pages** :
  - Allez dans **Pages** (section dans le menu de gauche).
  - Sous **Source**, sélectionnez la branche `main`.
  - Cliquez sur **Save**.
3. **URL du site générée** :  
  Votre site sera accessible à :  
  `https://<votre-utilisateur>.github.io/mon-site`.

---

## 5. Tester et mettre à jour le site

1. **Visitez l'URL générée** pour vérifier votre site.
2. **Pour mettre à jour le site** :
  - Modifiez vos fichiers localement.
  - Ajoutez les modifications :
    
    ```bash
    git add .
    ```
    
  - Committez les changements :
    
    ```bash
    git commit -m "Mise à jour"
    ```
    
  - Poussez les fichiers :
    
    ```bash
    git push
    ```
    
3. Les modifications seront visibles en ligne.

---

## Conseils supplémentaires

- Ajoutez des fichiers CSS ou JS pour enrichir votre site.
- Utilisez un éditeur de code comme **VSCode** pour une meilleure expérience.
- Explorez des frameworks comme **Bootstrap** pour un design plus professionnel.
- GitHub Pages prend également en charge **Jekyll** pour des sites statiques plus avancés.
