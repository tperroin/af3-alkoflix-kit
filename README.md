# Kit Arctic Fuse 3 + alkoFlix

Configuration « super Netflix » pour Kodi 21 : hubs Accueil / Films / Séries / Découvrir /
Ma liste, widgets alkoFlix et styles Stack / Ranked / Flyer.

## Contenu

| Fichier | Rôle |
|---|---|
| `repository.jurialmunkey-3.6.zip` | dépôt du skin Arctic Fuse 3 |
| `repository.alkoflix-1.0.1.zip` | dépôt alkoFlix |
| `resource.images.alkodicons.coal-1.0.3.zip` | icônes alkoFlix (optionnel) |
| `202611152015.zip` | configuration du skin à restaurer (15/11/2026) |

## Installation sur un nouvel appareil

1. Kodi 21.
2. Paramètres > Extensions > *Installer depuis un fichier zip* : les deux dépôts.
3. Installer **Arctic Fuse 3**, puis l'activer.
4. Installer **alkoFlix**, connecter Trakt et le débrideur.
5. Installer l'addon **Backup** (dépôt Kodi officiel > Programmes).
6. Copier `202611152015.zip` dans le dossier de sauvegarde de Backup
   (`special://profile/backup/` par défaut).
7. Backup > *Restaurer* > l'entrée datée du 15/11/2026 > cocher **addon_data**.
8. Confirmer si Kodi signale une version différente, puis redémarrer : les widgets se
   reconstruisent automatiquement.

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
