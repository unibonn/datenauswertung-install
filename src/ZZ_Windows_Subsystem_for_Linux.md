# Einrichten von Windows Subsystem für Linux

Unter Windows 10 und höher wird die Nutzung des WSL (Windows Subsystem for Linux) empfohlen. Hierbei sollte mindestens Windows 10 Build 19044 oder ein voll aktualisiertes Windows 11 verwendet werden, ab diesen Versionen unterstützt das aktuelle "WSL 2" auch grafische Anwendungen ohne teils komplizierte Modifikationen. Zudem sollte nach dem Aktualisieren ein aktuelles Linux installiert werden, falls zuvor bereits eine alte Linux-Umgebung installiert war.  
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
Bei einigen Linux-Versionen (z.B. Ubuntu) ist danach noch einmalig:
```shell
sudo apt update
```
nötig, damit weitere Paketinstallationen möglich sind, da die Paketlisten ansonsten nicht zur Verfügung stehen. In der Regel empfiehlt sich auch in der Linux-Umgebung zunächst eine volle Aktualisierung, also etwa bei Ubuntu / Debian:
```shell
sudo apt update && sudo apt dist-upgrade
```
