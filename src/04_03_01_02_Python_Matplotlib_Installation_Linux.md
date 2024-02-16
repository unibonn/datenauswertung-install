# Python/Matplotlib Installation unter Linux

Bei den meisten Linux-Systemen kommen vorinstallierte Python(3)-Module bei der OS-Installation mit.
Zum Aufsetzen einer virtuellen Umgebung, in die dann Matplotlib installiert werden kann, genügt in den meisten Fällen:
```shell
python -m venv <name-meiner-umgebung>
```

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