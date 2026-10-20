# Roll Egg's

Application web statique en français pour découvrir 100 idées de business, répondre à un questionnaire de 30 questions et obtenir des recommandations déterministes. Elle inclut aussi un catalogue filtrable, des favoris, un programme de 30 jours et un mini-CRM local.

## Fonctionnement

L'application est autonome dans `index.html` : aucun serveur ni étape de compilation n'est nécessaire. Les réponses, favoris, tâches, prospects et revenus sont conservés uniquement dans le navigateur via `localStorage`.

Elle charge cependant Tailwind CSS, Font Awesome et la police Plus Jakarta Sans depuis leurs CDN. Une connexion Internet est donc nécessaire pour obtenir la mise en forme et les icônes complètes.

## Lancer localement

Ouvrez simplement `index.html` dans un navigateur moderne. Pour un test plus proche de la mise en ligne, servez ce dossier avec n'importe quel serveur statique local.

## Déployer gratuitement avec GitHub Pages

1. Créez un dépôt GitHub public contenant les fichiers de ce dossier à sa racine, notamment `index.html`.
2. Sur GitHub, ouvrez **Settings** puis **Pages**.
3. Dans **Build and deployment**, choisissez **Deploy from a branch**.
4. Sélectionnez la branche `main` et le dossier `/(root)`, puis cliquez sur **Save**.
5. Attendez la publication : l'URL indiquée sur cette même page sera de la forme `https://<votre-compte>.github.io/roll-eggs/`.

Après chaque mise à jour envoyée sur `main`, GitHub Pages republie automatiquement l'application.

## Vérifications effectuées

- Les scripts inclus passent une vérification de syntaxe JavaScript.
- Le fichier contient 100 entrées de business et 30 questions.
- L'application ne requiert ni clé API ni données serveur.

## Limites connues

Les données sont propres à chaque navigateur et peuvent être effacées en supprimant les données du site. L'application ne synchronise pas les progrès entre appareils.
