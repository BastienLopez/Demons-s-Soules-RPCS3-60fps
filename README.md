# 📜 Installation de **Demon’s Souls (PS3)** sur **RPCS3**

## 1. Installer RPCS3

1. Télécharge l’archive officielle :  
   <https://rpcs3.net/download>
2. Décompresse dans un dossier sans accents ni espaces (ex. `C:\Emulateurs\RPCS3\`).
3. (Facultatif) Crée un raccourci de `rpcs3.exe` sur le bureau.

---

## 2. Installer le firmware PS3

1. Récupère **PS3 System Software Update** (section « Update using a computer ») :  
   <https://www.playstation.com/en-us/support/hardware/ps3/system-software/>
2. Lance **RPCS3** → **File ▸ Install Firmware**.  
3. Sélectionne le fichier `PS3UPDAT.PUP`.  
   > L’installation peut prendre quelques minutes. Patiente jusqu’au message « Successfully installed ».

---

## 3. Ajouter Demon's Souls

1. Télécharge ou rippe la version **EU (BLES-00932)** (~ 8,3 Go) :  
   <https://romsfun.me/download/demons-souls-34979/12/download_list_aff>  
   *(ou rippe ton propre disque avec un PS3 ISO Dumper)*  
2. Tu obtiens un dossier **`Demon's Souls [BLES-00932]`** contenant `PS3_GAME` et `PS3_DISC.SFB`.  
3. **Glisse-dépose** ce dossier dans la fenêtre RPCS3. Le jeu apparaît dans la liste.

---

## 4. Configurer les contrôles

1. **Pads ▸ Handler** → choisis ta manette (DualShock, XInput, etc.).  
2. Clique **Save**. Teste les boutons si besoin.

---

## 5. Appliquer les correctifs officiels RPCS3

1. Clic droit sur **Demon's Souls** → **Manage Game Patches**.  
2. Active :  
   - **Disable Motion Blur**  
   - **Unlock FPS** (60 FPS stables sur machines récentes)  
3. **Apply** puis **Save**.

---

## 6. Créer une configuration personnalisée

1. Clic droit → **Create Custom Configuration**.  
2. **GPU**  
   - **Resolution Scale** → choisis la résolution native de ton écran (ex. 150 % pour 1440p, 200 % pour 4K).  
   - **Additional Settings** → coche **Write Color Buffers** (corrige certains artefacts).  
3. Laisse les autres options par défaut, **Save**.

---

## 7. Installer les mods (optionnel mais vivement conseillé)

| Mod | Description rapide |
| --- | ------------------ |
| [DSfix-ish High Resolution Textures](https://www.nexusmods.com/demonssouls/mods/53) | Textures HD |
| [60 FPS Camera Patch](https://www.nexusmods.com/demonssouls/mods/27) | Caméra plus fluide |
| [Ascended Mod](https://www.nexusmods.com/demonssouls/mods/3) | Rééquilibrage & contenu QoL |
| [Re-translated UI](https://www.nexusmods.com/demonssouls/mods/11) | Interface FR/EN peaufinée |
| [No Depth-of-Field](https://www.nexusmods.com/demonssouls/mods/51) | Flou supprimé |
| [Improved Lighting](https://www.nexusmods.com/demonssouls/mods/57) | Lumière et couleurs revues |
| [Better Sounds](https://www.nexusmods.com/demonssouls/mods/8) | Effets audio HD |

### Installation des mods

1. Dans RPCS3, clic droit sur le jeu → **Open Folder ▸ Open Disc Game Folder** → ouvre `USRDIR`.  
2. Pour chaque mod :  
   - Ouvre le `.zip/.7z`, repère le dossier **`USRDIR`** ou les fichiers `.pkg`.  
   - **Glisse-dépose** le contenu à la racine de ton `USRDIR` existant.  
   - Accepte les remplacements si Windows demande.  
3. Une fois tous les mods copiés, ferme l’explorateur.

---

## 8. Premier lancement

1. Clique deux fois sur **Demon's Souls** dans RPCS3.  
2. Laisse le cache SPU/PPU se reconstruire (écran noir initial possible 1-2 min).  
3. Dans le jeu, règle la luminosité et vérifie que l’HUD, le framerate et les textures s’affichent comme prévu.

---

## 9. Conseils de performance

| Astuce | Effet |
| ------ | ----- |
| **Vsync off** dans RPCS3 | Réduit la latence mais peut entraîner du tearing |
| **Thread Scheduler** activé | Meilleure répartition CPU sur Intel/AMD récents |
| **SPU Decoder ▸ LLVM** | +FPS et moins de stutter après le pré-compil’ |

---


### FAQ éclair

- **Écran noir long au 1ᵉʳ boot ?** Normal, RPCS3 compile les shaders. Les relances seront instantanées.  
- **Crashs après un mod ?** Supprime-le du dossier `USRDIR`, vérifie qu’il est bien compatible avec la version EU.  
- **Sauvegardes ?** Elles se trouvent dans `dev_hdd0/home/00000001/savedata/`. Fais-en des copies régulières !

---

### Support & mises à jour

- **RPCS3** propose des builds quotidiennes : pense à mettre à jour (`Help ▸ Check for Updates`).  
- **Patches** : le gestionnaire affiche automatiquement les nouveaux correctifs RPCS3.  
- **Mods** : surveille l’onglet « Files » de chaque page NexusMods pour récupérer les dernières versions.
