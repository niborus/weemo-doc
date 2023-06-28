*************
Weemo's Minispiele
*************

.. note::
   In diesem Bereich werden nur die Minispiele erklärt, bei denen Einstellungen vorgenommen werden können.

.. _emojiquiz:

Emojiquiz
=========

Was ist das Emojiquiz?
^^^^^^^^^^^^^^^^^^^^^^

Das Emojiquiz ist - wie der Name bereits verrät - ein Minispiel wo man anhand von Emojis das Wort erraten muss.

Für jedes erratene Wort gibt es je nach Schwierigkeit Cornichon-Punkte.

Wie wird es eingerichtet?
^^^^^^^^^^^^^^^^^^^^^^^^^

- Es kann ein Kanal mit dem Namen `emojiquiz` erstellt werden.
- Möchtest du jedoch einen eigenen Namen festlegen, kannst du dieses mit ``/emojiquiz setchannel`` konfigurieren.

Es startet nicht, was soll ich tun?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- Gebe ``/emojiquiz settings`` ein und schaue nach, ob Weemo den Kanal aufgelistet hat.
- Überprüfe, ob Weemo die Berechtigungen **Nachrichten verwalten**, **Links einbetten** und **Reaktionen hinzufügen** hat.
- Falls Weemo die benötigten Berechtigungen hat, gebe ``/emojiquiz repair`` ein.

Was ist die Lösung zu diesem Emojiquiz?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- Unser Team verrät keine Lösungen aus dem Emojiquiz. Wenn dir ein Wort nicht einfällt, kannst du das aktuelle Emojiquiz mit dem Button ``Überspringen`` überspringen.

Was bedeuten die Reaktionen?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- ❌ bedeutet, dass du falsch liegst.
- ⭐ bedeutet, dass du sehr nah an dem gesuchten Begriff liegst.

.. _emojiquiz_befehle:

Befehle
^^^^^^^

.. csv-table::
    :widths: auto
    :align: left
    :header: "Befehl", "Beschreibung"

    "leaderboard emojiquiz", "Zeigt eine globale Top 10-Liste mit den meisten Punkten aller User an."
    "emojiquiz help", "Erklärt das Emojiquiz."
    "emojiquiz settings", "Zeigt die aktuellen Einstellungen."
    "emojiquiz setchannel", "Optional: Setzt den Kanal fest, in dem das Emojiquiz gespielt werden soll."
    "emojiquiz repair", "Repariert das Emojiquiz, sollte es nicht wie erwartet funktionieren."


.. _guessthenumber:

GuessTheNumber
=========

Spielprinzip
^^^^^^^^^^^^
Weemo sucht eine zufällige Zahl aus. Du musst versuchen, diese Zahl zu erraten.
Gelingt dir das, erhältst du einen Punkt und eine weitere Runde beginnt.

Befehle
^^^^^^^
.. csv-table::
    :widths: auto
    :align: left
    :header: "Befehl", "Beschreibung"

    "leaderboard guessthenumber", "Zeigt eine globale Top 10-Bestenliste der User, die die meisten Zahlen erraten haben."
    "guessthenumber setchannel [#Textkanal]", "Konfiguriert den Textkanal, in dem GuessTheNumber gespielt werden soll."
    "guessthenumber reset", "Entfernt den Textkanal, in dem GuessTheNumber gespielt werden soll."



.. _antonymquiz:

Antonymquiz
=========

Spielprinzip
^^^^^^^^^^^^
Weemo gibt dir einen zufälligen Begriff vor, dessen Antonym ("Gegenteil") du erraten musst.
Wenn du ein Antonym richtig erraten hast, erhälst du, je nach Schwierigkeitsstufe, eine gewisse Anzahl an Cornichon-Punkten.

Befehle
^^^^^^^
.. csv-table::
    :widths: auto
    :align: left
    :header: "Befehl", "Beschreibung"

    "leaderboard antonymquiz", "Zeigt eine globale Top 10-Bestenliste der User, die die meisten Antonyme erraten haben."
    "antonymquiz setchannel [#Textkanal]", "Konfiguriert den Textkanal, in dem Antonymquiz gespielt werden soll."
    "antonymquiz settings", "Zeigt die aktuellen Einstellungen an."
