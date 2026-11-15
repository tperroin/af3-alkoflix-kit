# Kit Arctic Fuse 3 + alkoFlix

Configuration « super Netflix » pour Kodi 21 : hubs Accueil / Films / Séries / Découvrir /
Ma liste, widgets alkoFlix et styles Stack / Ranked / Flyer.

## Contenu

| Fichier | Rôle |
|---|---|
| `repository.jurialmunkey-3.6.zip` | dépôt du skin Arctic Fuse 3 |
| `repository.alkoflix-1.0.1.zip` | dépôt alkoFlix |
| `resource.images.alkodicons.coal-1.0.3.zip` | icônes alkoFlix (optionnel) |
| `AF3-config.zip` | configuration du skin à restaurer |

## Installation sur un nouvel appareil

1. Kodi 21.
2. Paramètres > Extensions > *Installer depuis un fichier zip* : les deux dépôts.
3. Installer **Arctic Fuse 3**, puis l'activer.
4. Installer **alkoFlix**, connecter Trakt et le débrideur.
5. Installer l'addon **Backup** (dépôt Kodi officiel > Programmes).
6. Backup > *Restaurer* > `AF3-config.zip` > cocher **addon_data**.
7. Kodi redémarre : les widgets se reconstruisent automatiquement.

## Source Kodi

Ajouter `https://tperroin.github.io/af3-alkoflix-kit/` comme source dans
Paramètres > Gestionnaire de fichiers, puis *Installer depuis un fichier zip*.

## Notes

- Ne pas recopier `addon_data/plugin.video.alkoflix` entre appareils : reconnecter Trakt
  et le débrideur sur place.
- Skin Arctic Fuse 3 ≥ 3.5.1 requis.
- Le zip de config est au format de l'addon Backup (`xbmcbackup.val` + `addon_data`).
