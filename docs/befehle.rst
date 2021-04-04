*******
Befehle
*******

.. contents:: Inhalte

Befehle eingeben
================

Befehle werden eingegeben, indem man ``w#befehl Argumente`` eingibt.

``[Argument-Typ]`` ist ein notwendiges Argument,
``<Argument-Typ>`` ein optionales.

Übersicht
=========

Nützliches
^^^^^^^^^^

.. csv-table::
    :widths: auto
    :align: left
    :header: "Befehl", "Beschreibung"

    "userinfo <User>", "Zeigt Informationen über einen User an."
    "serverinfo", "Zeigt Informationen über den Server an."
    "roleinfo [Rolle]", "Zeigt Informationen über eine Rolle an."
    "channelinfo [#Kanal]", "Zeigt Informationen über einen Kanal an."
    "emoteurl [Emoji]", "Zeigt die URL eines Custom-Emojis an, mit dem man das Emoji herunterladen kann."
    "avatar <User>", "Zeigt das Profilbild eines Users an."
    "color [Farbcode]", "Zeigt die Farbe an."
    "randomcolor", "Zeigt eine zufällige Farbe an."
    "ping", "Misst den Ping / die Latenz von Weemo."
    "poll [Frage] <noembed>", "Erstellt eine Umfrage."
    "`tag`_", "Speichern und ausfrufen von kurzen Texten."
    "random [a] [b]", "Würfelt eine Zahl, die zwischen a und b liegt. (Einschließlich a, aber ohne b)"
    "`remindme`_ [Zeitangabe] [Erinnerung]", "Erstellt eine Erinnerung."

Fun
^^^

.. csv-table::
    :widths: auto
    :align: left
    :header: "Befehl", "Beschreibung"

    "cookie <eat>", "Kekse |cookie|"
    "coinflip", "Wirft eine Münze."
    "rps", "Spiele *Schere, Stein, Papier*"
    "dog", "Sende ein Hundebild. |dog|"
    "cat", "Sende ein Katzenbild. |cat|"
    "`count`_", "Konfiguriert den Channel, in dem gezählt werden soll."
    "marry [@User]", "Stelle einen Heiratsantrag. |ring|"
    "divorce", "Lass dich scheiden. |broken_heart|"
    "meme", "Sende ein Meme."

Details
=======

tag
^^^

Tags können genutzt werden, um kurze Textabschnitte zu speichern und schnell wieder aufzurufen.
Dies ist praktisch, falls auf eurem Server häufig die selbe Frage gestellt wird, und ihr nicht jedes mal einen neuen
Antworttext schreiben wollt.

.. csv-table::
    :widths: auto
    :align: left
    :header: "Befehl", "Beschreibung"

    "tag", "Listet alle Tags für diesen Server auf"
    "tag [Tag] <@User>", "Ruft den Tag auf und pingt auch bei einem erwähnten Mitglied."
    "tag create [Tag] [Nachricht]", "Erstellt einen neuen Tag mit dem Namen und der hinterlassenden Nachricht."
    "tag edit [Tag] [Nachricht]", "Editiert einen Tag."
    "tag info [Tag]", "Ruft Informationen über den Tag ab."
    "tag rename [Tag] [Neuer |nbsp| Tagname]", "Benennt den angegebenen Tag um."
    "tag delete [Tag]", "Löscht einen Tag aus der Liste."

remindme
^^^^^^^^

Erstellt Erinnerungen. Es ist nur eine Erinnerung zeitgleich pro Account möglich.

.. csv-table::
    :widths: auto
    :align: left
    :header: "Befehl", "Beschreibung"

    "remindme [Zeitangabe] [Erinnerung]", "Startet eine neue Erinnerung."
    "remindme remove", "Stoppt die aktuelle Erinnerung."

**Beispiel**: ``w#remindme 30m Müll rausbringen``

**Zeitangaben**:

.. csv-table::
    :widths: auto
    :align: left

    "``s``", "Sekunden"
    "``m``", "Minuten"
    "``d``", "Tage"
    "``mo``", "Monate"

count
^^^^^

.. csv-table::
    :widths: auto
    :align: left
    :header: "Befehl", "Beschreibung"

    "count setchannel [#Textkanal]", "Konfiguriert den Textkanal, in dem gezählt werden soll. Sollte der Textkanal nicht das erste mal eingerichtet werden sondern gewechselt, wird der Zähler auf 1 zurückgesetzt."
    "count removechannel", "Entfernt den Textkanal wieder."



.. |cookie| unicode:: 0x1f36a .. Keks Emoji
.. |cat| unicode:: 0x1f431 .. Katzen Emoji
.. |dog| unicode:: 0x1f436 .. Hunde Emoji
.. |coin| unicode:: 0x1fa99 .. Münze Emoji
.. |ring| unicode:: 0x1f48d .. Ehering Emoji
.. |broken_heart| unicode:: 0x1f494 .. Gebrochenes Herz Emoji
.. |nbsp| unicode:: 0xA0 .. Non breaking Space
   :trim:
