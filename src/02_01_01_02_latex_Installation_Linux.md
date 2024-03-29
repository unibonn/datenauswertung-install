# LaTeX Installation unter Linux

Auf den meisten Linux-Systemen befindet sich LaTeX in den Standard-Paketquellen. Das bedeutet, dass sich LaTeX (sowie spätere Updates) als Bestandteil des Systems installieren lassen. 

Dies geschieht je nach Linux-Distribution leicht anders, siehe auch [Paketverwaltungen auf Linux](./ZZ_Paketverwaltungen_Linux.md). Bei den verbreitesten Distributionen, die auf Debian basieren (dazu gehören auch Ubuntu und Linux Mint), kann entweder ein grafisches Software-Center verwendet werden, oder alternativ das Kommando:
```shell
sudo apt install texlive-full
```
Dies installiert LaTeX ohne grafische Oberfläche.
Falls eine Umgebung mit grafischer Oberfläche gewünscht ist, lässt sich eine solche über
```shell
sudo apt install texstudio
```
installieren.
