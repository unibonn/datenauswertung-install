# Installation von ROOT unter Windows

Unter Windows 10 und höher wird die Nutzung des WSL (Windows Subsystem for Linux) empfohlen. Hierbei sollte mindestens Windows 10 Build 19044 oder ein voll aktualisiertes Windows 11 verwendet werden, ab diesen Versionen unterstützt das aktuelle "WSL 2" auch grafische Anwendungen ohne teils komplizierte Modifikationen. Zudem sollte nach dem Aktualisierungen ein aktuelles Linux installiert werden, falls zuvor bereits eine alte Linux-Umgebung installiert war.  
Der verwendete Windows-Build kann mit folgendem Kommando geprüft werden:
```
winver.exe
```
Die verwendete WSL-Version für installierte Linux-Systeme kann wie folgt geprüft werden:
```
wsl --list --verbose
```
Falls sich dabei herausstellt, dass WSL noch nicht installiert ist, kann es mit dem Kommando:
```
wsl --install
```
aktiviert werden.
Ein Update von WSL ist wie folgt möglich (in einer Eingabeaufforderung / PowerShell mit Administratorrechten):
```
wsl --update
wsl --shutdown
```
Ist schlussendlich ein aktuelles Linux-System in einer aktuellen WSL-Umgebung installiert, müssen vor der Installation von ROOT zunächst ein paar Abhängigkeiten, die auch für die Auswertung sinnvoll sind, innerhalb der Linux-Umgebung nachinstalliert werden:
```bash
sudo apt update && sudo apt dist-upgrade
sudo apt install build-essential libtbb-dev libtiff5 x11-apps git
```
Schlussendlich kann den normalen Instruktionen für eine Installation unter Linux gefolgt werden, also herunterladen des Tarballs von der ROOT Webseite (mit wget), dann entpacken. Wichtig ist, tatsächlich in der Ubuntu-Umgebung mit wget herunterzuladen und zu entpacken, beim Herunterladen und Entpacken unter Windows und nachträglicher Kopie in die Linux-Umgebung kann es zu Problemen kommen, da Windows die Dateien unnötigerweise konvertiert. Schlussendlich dann in der Ubuintu-Umgebung folgendes Kommando ausführen:
```bash
source root/bin/thisroot.sh
```
