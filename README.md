# Générateur de configurations

Outil pour transformer un modèle de configuration réseau en config prête à coller,
en ne remplissant que les variables. Une seule page HTML, **sans installation** et
**100 % local** : tout se passe dans le navigateur, aucune donnée n'est envoyée nulle part.

## Utilisation

- **En local** : ouvrir `index.html` dans un navigateur (double-clic).
- **En ligne** (si GitHub Pages est activé) : voir le lien dans l'onglet *Settings → Pages*.

## Fonctions

- Modèles réutilisables avec variables entre doubles accolades, ex. `{{ nom du site }}` — l'outil
  détecte les variables et crée les champs automatiquement.
- **Une config** : remplissage champ par champ, génération en direct.
- **En lot** : coller des lignes depuis Excel, une config par ligne.
- **Lien P2P** : génère les deux bouts d'un lien d'un coup (IP voisine calculée sur le /31,
  MEP source/remote inversés, maintenance-association partagée), en unitaire ou par lot.
- **Validation** des @IP et des MEP (champ en rouge si invalide).
- **Détection de collisions** sur les lots de liens (@IP en double, interface réutilisée).
- **Import / export** des modèles en `.json` pour partager le même jeu à toute l'équipe.

Les modèles sont enregistrés dans le navigateur de chaque utilisateur (localStorage).

## Modifier un modèle

Dans l'outil : bouton **✎ Modifier** → éditer le texte → **Enregistrer**.
Inutile de toucher au code : l'édition passe par l'interface.

## Confidentialité

L'outil ne communique avec aucun serveur. En revanche, le **contenu des modèles est inscrit
dans le fichier HTML** : si le dépôt est public, ces modèles sont lisibles par tout le monde.
Pour de l'outillage interne, préférer un dépôt **privé** (ou un Git interne) et ne jamais
committer de clés, mots de passe ou secrets réels dans les modèles par défaut.

---

Outil interne — fonctionne hors ligne, aucune donnée transmise.
