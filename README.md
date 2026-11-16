# Kit Arctic Fuse 3 + alkoFlix

Configuration « super Netflix » pour Kodi 21 : hubs Accueil / Films / Séries / Découvrir /
Ma liste, widgets alkoFlix et styles Stack / Ranked / Flyer.

## Contenu

| Fichier | Rôle |
|---|---|
| `repository.jurialmunkey-3.6.zip` | dépôt du skin Arctic Fuse 3 |
| `repository.alkoflix-1.0.1.zip` | dépôt alkoFlix |
| `resource.images.alkodicons.coal-1.0.3.zip` | icônes alkoFlix (optionnel) |
| `202611161905.zip` | config **allégée** : 20 widgets, 12 éléments par widget (TV 2 Go) |
| `202611152015.zip` | config **complète** : 47 widgets, 20 éléments par widget (box musclée) |

Les deux archives contiennent les mêmes hubs, styles et réglages : seule la quantité de
widgets change. Sur une TV Android d'entrée de gamme, prendre l'allégée, sinon le premier
chargement sature la mémoire et Kodi se fait tuer par le système.

## Installation sur un nouvel appareil

1. Kodi 21.
2. Paramètres > Extensions > *Installer depuis un fichier zip* : les deux dépôts.
3. Installer **Arctic Fuse 3**, puis l'activer.
4. Installer **alkoFlix**, connecter Trakt et le débrideur.
5. Installer l'addon **Backup** (dépôt Kodi officiel > Programmes).
6. Copier l'archive choisie dans le dossier de sauvegarde de Backup
   (`special://profile/backup/` par défaut).
7. Backup > *Restaurer* > l'entrée datée (16/11/2026 pour l'allégée) > cocher **addon_data**.
8. Confirmer si Kodi signale une version différente, puis quitter Kodi complètement et le
   relancer. Le premier chargement des widgets prend plusieurs minutes, ne pas toucher la
   télécommande.

## Source Kodi

Ajouter `https://tperroin.github.io/af3-alkoflix-kit/` comme source dans
Paramètres > Gestionnaire de fichiers, puis *Installer depuis un fichier zip*.

## Notes

- Ne pas recopier `addon_data/plugin.video.alkoflix` entre appareils : reconnecter Trakt
  et le débrideur sur place.
- Skin Arctic Fuse 3 ≥ 3.5.1 requis.
- Le zip de config est au format de l'addon Backup (`xbmcbackup.val` + `addon_data`).
- Le nom du zip fait partie du format : Backup ne liste que les archives dont le nom
  commence par 12 chiffres (`AAAAMMJJhhmm`), et le dossier interne doit porter exactement
  le même nom que l'archive. Renommer le fichier casse la restauration.
- Pour alléger encore : renommer en `.json.off` les fichiers
  `skinvariables-shortcut-*widgets.json` dans
  `addon_data/script.skinvariables/nodes/skin.arctic.fuse.3/`, puis relancer Kodi.
