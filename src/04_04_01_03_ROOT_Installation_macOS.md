# Installation von ROOT unter macOS

Unter macOS lässt sich ROOT über mehrere Wege installieren:

- Über eine Paketverwaltung wie Homebrew, Macports oder Nix. Weitere Details dazu sind unter folgender Adresse zu finden:
  https://root.cern/install/#macos-package-managers
- Über Conda wie weiter unten beschrieben.

Bei der späteren Auswertung muss auf macOS Systemen das Makefile leicht angepasst werden. Hier muss die Option:
```
-Wl,--no-as-needed
```
entfernt werden, die auf Ubuntu-Systemen benötigt (und auf anderen Systemen ignoriert) wird, aber auf macOS zwar nicht benötigt ist, allerdings zu einer Fehlermeldung führt.
