# Installation von ROOT unter Windows

Zunächst muss das Windows Subsystem für Linux wie [hier](./ZZ_Windows_Subsystem_for_Linux.md) beschrieben installiert werden.
Ist schlussendlich ein aktuelles Linux-System in einer aktuellen WSL-Umgebung installiert, müssen vor der Installation von ROOT zunächst ein paar Abhängigkeiten, die auch für die Auswertung sinnvoll sind, innerhalb der Linux-Umgebung nachinstalliert werden:
```bash
sudo apt update && sudo apt dist-upgrade
sudo apt install build-essential libtbb-dev libtiff5 x11-apps git
```
Schlussendlich kann den normalen Instruktionen für eine Installation unter Linux gefolgt werden, also herunterladen des Tarballs von der ROOT Webseite (mit `wget`), dann entpacken. Wichtig ist, tatsächlich in der Ubuntu-Umgebung mit `wget` herunterzuladen und zu entpacken, beim Herunterladen und Entpacken unter Windows und nachträglicher Kopie in die Linux-Umgebung kann es zu Problemen kommen, da Windows die Dateien unnötigerweise konvertiert. Schlussendlich dann in der Ubuintu-Umgebung folgendes Kommando ausführen:
```bash
source root/bin/thisroot.sh
```

Unter den [Ersten Schritten](./04_04_02_ROOT_Erste_Schritte.md) mit ROOT finden sich auch noch einige, zum Teil betriebssystemabhängig, Hinweise zur allgemeinen Nutzung und Konfiguration.
