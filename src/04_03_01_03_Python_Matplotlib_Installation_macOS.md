# Python/Matplotlib Installation unter macOS

Bei den meisten macOS-Versionen kommen vorinstallierte Python-3-Module mit.
Zum Aufsetzen einer virtuellen Umgebung, in die dann Matplotlib installiert werden kann, genügt in den meisten Fällen:
```shell
python3 -m venv <name-meiner-umgebung>
```
Sollte das Aufsetzen der Umgebung mit `python3` nicht funktionieren, ist in den meisten Fällen eine veraltete macOS-Version installiert, welche eine ältere Python-Version beinhaltet.
In diesem Fall sollte eine neuere Python-Version über die vorgestellten [Paketverwaltungen](./ZZ_Paketverwaltungen_macOS.md) installiert werden, z.B.:
```shell
brew install python@3.11
```
Danach sollte die virtuelle Umgebung wie beschrieben erstellt werden können.

Sobald diese Umgebung erstellt ist, kann man sie starten bzw. in die Umgebung wechseln, indem man den folgenden Befehl ausführt:
```shell
source <name-meiner-umgebung>/bin/activate
```

Danach kann Matplotlib über den bereits beschrieben Weg installiert werden:
```shell
pip install matplotlib
```

Um die Arbeit zu einem späteren Zeitpunkt wieder aufzunehmen, genügt es, wieder in die erstellte Umgebung zu wechseln.
Matplotlib steht dann automatisch wieder zur Verfügung.
