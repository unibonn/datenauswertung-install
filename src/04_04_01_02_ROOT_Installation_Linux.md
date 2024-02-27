# Installation von ROOT unter Linux

Hier hängt der praktischste Weg von der verwendeten Linux-Distribution ab. Bei einigen Distributionen steht root direkt in den Paketquellen zur Verfügung und kann über die Paketverwaltung installiert werden:
[https://repology.org/project/root/versions](https://repology.org/project/root/versions)

Dies betrifft hauptsächlich RedHat-basierte Distributionen, ArchLinux und Gentoo. Für Ubuntu Linux in den LTS-Versionen stellt das root-Team selbst vorkompilierte Pakete zur Verfügung, die nach der Anleitung unter
[https://root.cern/install/](https://root.cern/install/)
installiert werden können. Wichtig dabei ist, die passende Version herunterzuladen (etwa "Ubuntu 20" für Ubuntu 20.04 LTS).

Wenn auf diesen Wegen keine Version zur Verfügung steht, bleibt eine Installation über [Conda](https://root.cern/install/#conda) oder "selbst kompilieren", was allerdings eine größere Herausforderung darstellt.
Für die Installation über Conda muss auf dem System zum Beispiel entweder [Miniconda](https://docs.anaconda.com/free/miniconda/index.html) oder [Anaconda](https://docs.anaconda.com/free/anaconda/) installiert sein.
Diese sind meist Teil der Standard-Paketquellen.

