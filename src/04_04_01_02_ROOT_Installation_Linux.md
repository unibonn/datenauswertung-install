# Installation von ROOT unter Linux

Hier hängt der praktischste Weg von der verwendeten Linux-Distribution ab. Bei einigen Distributionen steht `root` direkt in den Paketquellen zur Verfügung und kann über die Paketverwaltung installiert werden:
[https://repology.org/project/root/versions](https://repology.org/project/root/versions)

Dies betrifft hauptsächlich RedHat-basierte Distributionen, ArchLinux und Gentoo. Für Ubuntu Linux in den LTS-Versionen stellt das ROOT-Team selbst vorkompilierte Pakete zur Verfügung, die nach der Anleitung unter
[https://root.cern/install/](https://root.cern/install/)
installiert werden können. Wichtig dabei ist, die passende Version herunterzuladen (etwa "Ubuntu 24.04" für Ubuntu 24.04 LTS).
Außerdem müssen noch weitere benötigte Pakete selbstständig installiert werden, eine vollständige Liste inklusive des Befehls zum installieren sind [hier](https://root.cern/install/dependencies/#ubuntu-and-other-debian-based-distributions) zu finden.

Wenn auf diesen Wegen keine Version zur Verfügung steht, bleibt eine Installation über [Miniforge](https://github.com/conda-forge/miniforge) oder "selbst kompilieren", was allerdings eine größere Herausforderung darstellt.
Eine Installation über Miniforge kann folgendermaßen durchgeführt werden:
```bash
# Eigentliche Installation von Miniforge
wget "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
bash Miniforge3-$(uname)-$(uname -m).sh -b -p ~/miniforge
# Erstellen einer virtuellen Umgebung inklusive der ROOT-Installation
source ~/miniforge/etc/profile.d/conda.sh
conda create -n my_root_env root root_base
```

Nach erfolgreicher Installation kann ROOT dann über den folgenden Weg "geladen" werden:
```bash
source ~/miniforge/etc/profile.d/conda.sh
conda activate my_root_env
```

Unter den [Ersten Schritten](./04_04_02_ROOT_Erste_Schritte.md) mit ROOT finden sich auch noch einige, zum Teil betriebssystemabhängige, Hinweise zur allgemeinen Nutzung und Konfiguration.
