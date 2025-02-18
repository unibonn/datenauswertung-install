# Installation von ROOT unter macOS

Unter macOS lässt sich ROOT über mehrere Wege installieren:

- Über eine [Paketverwaltung](./ZZ_Paketverwaltungen_macOS.md) wie Homebrew, Macports oder Nix. Weitere Details dazu sind auf der [ROOT-Webseite](https://root.cern/install/#macos-package-managers) zu finden.
- Über Conda wie ebenfalls auf der [ROOT-Webseite](https://root.cern/install/#conda) beschrieben. Dazu kann zum Beispiel [Miniforge](https://github.com/conda-forge/miniforge) über Homebrew unter dem Paketnamen `miniforge` installiert werden.

Falls der Weg über Miniforge gewählt wurde, ist es zu empfehlen, einen Installationsort abweichend von `/opt/homebrew` anzugeben. Der Hintergrund dazu ist, dass Updates von Miniforge ansonsten dazu führen können, dass unter `/opt/homebrew` erstellte Environments gelöscht werden.
Folgender Befehl würde z.B. ein ROOT-Environment im eigenen Home im Unterordner `my_root_env` anlegen:
```bash
conda create -p ~/my_root_env root root_bas
```
Zum späteren Aktivieren des Environments ist zu beachten, dass der volle Pfad angegeben werden muss:
```bash
conda activate ~/my_root_env
```

Unter den [Ersten Schritten](./04_04_02_ROOT_Erste_Schritte.md) mit ROOT finden sich auch noch einige, zum Teil betriebssystemabhängige, Hinweise zur allgemeinen Nutzung und Konfiguration.
