Pygame Zero installieren
========================

Desktop
-------

Die Installation von **Python 3** ist Vorraussetzung für die Installation von Pygame Zero.
Bei **Linux** oder **Raspberry Pi** ist dies bereits vorinstalliert. Für andere Betriebssysteme
kann Python 3 unter `<https://www.python.org/>` heruntergeladen werden.

Generell empfiehlt sich die Installation mithilfe von Pythons Paketverwaltungsprogramm **pip**.

Windows und Mac
'''''''''''''''
::

    pip install pgzero


Linux
'''''

::

   sudo pip install pgzero


Bei der Fehlermedlung ``sudo: pip: command not found`` kann folgender Befehl hilfreich sein::

    sudo pip3 install pgzero

Beispiel: Installation in Thonny
''''''''''''''''''''''''''''''''

Einige IDEs (gerade für Anfänger) bieten bereits einfache grafische Oberflächen zur Installation von neuen Paketen (s. Thonny unten).

.. image:: _static/thonny_pgzero_install.jpg

Pygame Zero in IDLE, Mu, Thonny und anderen IDEs
------------------------------------------------

Pygame Zero ausführen
'''''''''''''''''''''

Um Pygame Zero in einem Python Programm zu verwenden, muss folgender Code eingefügt werden:

In der ersten Zeile:

::

    import pgzrun

In der letzten Zeile:


::

    pgzrun.go()

Hinweis: In Thonny kann mittels des Pygame Zero Modus auf diese beiden Zeile verzichtet werden. Um diesen Modus zu aktivieren,
muss im Menü > Ausführen > Pygame Zero Modus aktiviert werden.

Beispiel
''''''''


::

    import pgzrun


    WIDTH = 800
    HEIGHT = 600

    def draw():
        screen.clear()
        screen.draw.circle((400, 300), 30, 'white')


    pgzrun.go()

Dieser Code kann einfach in eine beliebige IDE kopiert werden.

Beliebte IDEs für Anfänger sind (neben der Standard-IDE **IDLE**) **Mu** und **Thonny**:

* **Mu**: `<https://codewith.mu/>`

* **Thonny**: `<https://thonny.org/>`

Beispiel in Thonny
''''''''''''''''''

.. image:: _static/thonny_pgzero_example.jpg
