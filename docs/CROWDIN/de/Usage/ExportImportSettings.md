# Export & import settings

## Quand dois-je exporter les paramètres ?

Préparez-vous aux imprévus. Vous pouvez modifier des paramètres importants par accident et avoir des problèmes pour annuler les modifications. Votre téléphone pourrait se casser ou être volé. Pour revenir facilement à l'état où vous étiez, les paramètres doivent être exportés régulièrement.

La meilleure pratique consiste à exporter les paramètres après un changement ou la réalisation d'un objectif.

Les paramètres exportés doivent être copiés sur un stockage cloud ou sur votre ordinateur, c'est mieux si vous utilisez deux emplacements différents. Ainsi vous serez prêt en cas de perte ou de dommages de votre téléphone AAPS et vous ne serez pas obligé de tout recommencer à partir de zéro.

Sur un ordinateur Windows 10, cela ressemble à ceci :

```{image} ../images/AAPS_ExImportSettingsWin.png
:alt: AndroidAPS Préférences téléphone connecté à l'ordinateur
```

## Informations exportées

Entre autres, les informations suivantes font partie des paramètres exportés :

- [Automation](../Usage/Automation.md) events
- [Config builder](../Configuration/Config-Builder.md) settings
- [Local profile](../Configuration/Config-Builder.md#local-profile) settings
- [Objectives](../Usage/Objectives.md) status incl. [exam results](../Usage/Objectives.md#objective-3-prove-your-knowledge)
- [Preferences](../Configuration/Preferences.md) incl. [NS Client settings](../Configuration/Preferences.md#nsclient)

## Format de sauvegarde chiffré

Settings backup is encrypted by a master password that can be set in [Preferences](../Configuration/Preferences.md#master-password) .

## Exporter les paramètres

- Hamburger menu (top left corner of screen)
- Maintenance
- Exporter les paramètres

```{image} ../images/AAPS_ExportSettings1.png
:alt: AndroidAPS exporter les paramètres 1
```

- Date and time of export will be added to the file name automatically and displayed together with the path.
- Click 'OK'.
- Enter [master password](../Configuration/Preferences.md#master-password) and click 'OK'.
- Successful export will be prompted at bottom of the screen.

```{image} ../images/AAPS_ExportSettings2.png
:alt: AndroidAPS exporter les paramètres 2
```

## Importer les paramètres

**Do not import settings while on an active Pod session** - see [Omnipod page for details](../Configuration/OmnipodEros.md#import-settings-from-previous-aaps).

- Hamburger menu (top left corner of screen)
- Maintenance
- Importer les paramètres

```{image} ../images/AAPS_ImportSettings1.png
:alt: AndroidAPS importer les paramètres 1
```

- All files from folder AAPS/preferences/ on your phone will be shown in the list.
- Select file.
- Confirm import by clicking 'OK'.
- Enter [master password](../Configuration/Preferences.md#master-password) and click 'OK'.

```{image} ../images/AAPS_ImportSettings2.png
:alt: AndroidAPS importer les paramètres 2
```

- Details on the preference file will be shown.
- Last option to cancel import.
- Click 'Import'.
- Confirm message by clicking 'OK'.
- AAPS will be restarted in order to activate imported preferences.

### Remarque pour les utilisateurs de Dana RS

- Comme les paramètres de connexion de la pompe sont également importés dans AAPS sur votre nouveau téléphone, il va déjà "connaître" la pompe et donc ne démarrera pas une analyse bluetooth.
- Please pair new phone and pump manually.

### Importer les paramètres des versions précédentes (avant AAPS 2.7)

- The "old" settings file (called 'AndroidAPSPreferences' - without file extension) must be in root folder of your smartphone (/storage/emulated/0).
- Do not put the "old" file in the same folder as the new exported settings (AAPS/preferences).
- You will find the "old" file on the bottom of the list in the import dialogue.

## Transférer les paramètres

- Best way to transfer settings file to a new phone is via USB cable or cloud service (i.e. Google Drive). Google Drive).
- Manuals can be found on the web, i.e. [Android help pages](https://support.google.com/android/answer/9064445?hl=en).
- If you experience problems with the transferred file try another way to transfer file.
