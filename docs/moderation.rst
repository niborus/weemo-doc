.. _moderation:

==========
Moderation
==========

Befehle
=======

Folgende Befehle sind  für Moderatoren.
Um diese auszuführen, benötigen Mitglieder entweder die Moderator\*innen-Rolle oder
müssen über ein entsprechendes Recht bei Discord verfügen.

.. _moderation_ban:

ban
^^^

Syntax: ``w#ban [@Mitglied] [Grund]``

Bannt ein Mitglied dauerhaft vom Server.
Sofern Weemo dem Mitglied eine DM schicken kann, wird der Grund für den Ban an das Mitglied gesendet.
Das Mitglied kann nach einem Ban dem Server nicht wieder beitreten.
Dies löscht alle neueren Nachrichten des Mitglieds.

.. _moderation_idban:

idban
^^^^^

Syntax: ``w#idban [ID] [Grund]``

Bannt eine Nutzerin / einen Nutzer dauerhaft vom Server.
Die Person kann nach einem Ban dem Server nicht beitreten.
Der Befehl kann auch auf Personen angewandt werden, die den Server bereits verlassen oder noch nie betreten haben.
Dies löscht alle neueren Nachrichten der Person.
Dazu wird die :ref:`ID<id>` der Person benötigt.

.. _moderation_tempban:

tempban
^^^^^^^

Syntax: ``w#tempban [@Mitglied] [Dauer] [Grund]``

Bannt eine Nutzerin / einen Nutzer für die angegebene Zeit vom Server.
Nach Ablauf der Zeit, wird das Mitglied entbannt.
Dies löscht alle neueren Nachrichten des Mitglieds.

.. _moderation_unban:

unban
^^^^^

Syntax: ``w#unban [ID]``

Entbannt eine gebannte Person.
Dazu wird die :ref:`ID<id>` der Person benötigt.

.. _moderation_mute:

mute
^^^^

Syntax: ``w#mute [@Mitglied] [Dauer] <Grund>``

Gibt einem Mitglied für die angegebene Dauer die Mute-Rolle und
verweigert dem Mitglied auf diese Weise das schreiben und sprechen.


.. _moderation_unmute:

unmute
^^^^^^

Syntax: ``w#unmute [@Mitglied]``

Entfernt die Mute-Rolle vom Mitglied.

.. _moderation_kick:

kick
^^^^

Syntax: ``w#kick [@Mitglied] [Grund]``

Alias: ``raus``

Entfernt ein Mitglied vom Server.
Sofern Weemo dem Mitglied eine DM schicken kann, wird der Grund für den Kick an das Mitglied gesendet.
Das Mitglied kann nach einem Kick den Server wieder beitreten.
Dies löscht keine Nachrichten des Mitglieds.

.. _moderation_warn:

warn
^^^^

Syntax: ``w#warn [@Mitglied] [Grund]``

Verwarnt ein Mitglied.
Sofern Weemo dem Mitglied eine DM schicken kann, wird der Grund für die Verwarnung an das Mitglied gesendet.
Verwarnungen werden gespeichert und können mit punishments_ von Moderator\*innen abgerufen werden.

.. _moderation_purge:

purge
^^^^^

Syntax: ``w#purge [Anzahl]``

Alias: ``cc``

Löscht die letzten Nachrichten in einem Kanal.
Die ``Anzahl`` der zu löschenden Nachrichten muss zwischen zwei und 100 liegen.

Nachrichten, die zu alt sind, können nicht von Weemo gelöscht werden.

.. _moderation_punishments:

punishments
^^^^^^^^^^^

Syntax: ``w#punishments <Mitglied>``

Zeigt die Verwarnungen eines Mitglieds an.


Syntax: ``w#punishments id <ID>``

Zeigt die Verwarnung mit der angegebenen ID an.


.. _modlog:

Modlog
======

Das Modlog speichert Ereignisse ab, die auf dem Server passieren.
Es speichert gelöschte und geänderte Nachrichten, was der Automod gelöscht hat, wer verwarnt wurde und warum,
wann welche Einstellungen geändert wurden und vieles mehr.
Dies ist für Moderator\*innen nützlich, um gelöschte Beleidigungen oder veränderte Gespräche nachzuvollziehen.

Der Modlog sollte ein eigener Textkanal sein, kann aber mit dem Log anderer Bots kombiniert werden.
Wir empfehlen, den Modlog zu einem privatem Kanal zu machen, auf den nur Moderator\*innen zugriff haben.

Einstellungen
^^^^^^^^^^^^^

Mit ``w#modlog setchannel [logchannel]`` kann ein Textkanal als Modlog-Kanal eingestellt werden.

Eine Übersicht, welche Module aktiv sind, kann mit ``w#modlog`` abgefragt werden.
Durch die eingabe von ``w#modlog``, gefolgt von der Nummer den Moduls in einer zweiten Nachricht,
kann eine Modul aktiviert/deaktiviert werden.

Es exestieren folgende Module:

+--------+-----------------------------+------------------------------------------+
| Nummer | Log für                     | Beinhaltet                               |
+========+=============================+==========================================+
|      1 | Gilden                      | - Serverregion aktualisiert              |
|        |                             | - Serverinhaber\*in gewechselt           |
|        |                             | - Servername geändert                    |
|        |                             | - Servericon geändert                    |
|        |                             | - Verifizierungsstufe verändert          |
|        |                             | - Mitglied gebannt                       |
|        |                             | - Mitglied entbannt                      |
|        |                             | - moderativer Befehl ausgeführt          |
+--------+-----------------------------+------------------------------------------+
|      2 | Sprachkanal                 | - Sprachkanal betreten                   |
|        |                             | - Sprachkanal verlassen                  |
|        |                             | - Sprachkanal gewechselt                 |
|        |                             | - Sprachkanal erstellt                   |
|        |                             | - Sprachkanal gelöscht                   |
+--------+-----------------------------+------------------------------------------+
|      3 | Textkanal                   | - Textkanal erstellt                     |
|        |                             | - Textkanal gelöscht                     |
|        |                             | - Sprachkanal erstellt                   |
|        |                             | - Sprachkanal gelöscht                   |
+--------+-----------------------------+------------------------------------------+
|      4 | Bearbeitete Nachrichten     | - Mitglied hat eine Nachricht bearbeitet |
+--------+-----------------------------+------------------------------------------+
|      5 | Server betreten & verlassen | - Mitglied hat den Server betreten       |
|        |                             | - Mitglied hat den Server verlassen      |
+--------+-----------------------------+------------------------------------------+
|      6 | Rollen                      | - Rolle erhalten                         |
|        |                             | - Rolle entfernt                         |
|        |                             | - Rolle erstellt                         |
|        |                             | - Rolle gelöscht                         |
+--------+-----------------------------+------------------------------------------+
|      7 | Nachrichten gelöscht        | - Mitglied hat Nachricht gelöscht        |
+--------+-----------------------------+------------------------------------------+
|      8 | Mitglieder                  | - Nickname geändert                      |
+--------+-----------------------------+------------------------------------------+

.. _automod:

Automod
=======

.. csv-table::
    :widths: auto
    :align: left
    :header: "Befehl", "Beschreibung"

    "automod toggle", "Aktiviert oder deaktiviert den AutoMod."
    "automod filter", "Zeigt die Wörter/Dateiendungen, die vom AutoMod erfasst werden."

Wortfilter
^^^^^^^^^^

Der Wortfilter schlägt an, falls eines der Wörter in einer Nachricht vorkommt. Es reicht, wenn das Wort als Teil eines
anderen Wortes vorkommt. So wird das Wort "but" auch in dem Wort "Butter" erkannt.

Mit ``w#automod filter add [Wort]`` und ``w#automod filter remove [Wort]`` können Wörter hinzugefügt und entfernt
werden.

Dateifilter
^^^^^^^^^^^

Der Dateifilter löscht Nachrichten mit Anhängen, die eine bestimmte Dateiendung haben.
Standardmäßig sind einige Dateiendungen die häufig für Schadsoftware verwendet werden (wie ``.exe`` oder ``.sh``)
bereits eingerichtet.

.. warning:: Weemo hat keinen Virenscaner. Dateien die vom Automod nicht erfasst werden, können trotzdem Schadsoftware enthalten.

Der Dateifilter kann mit ``w#automod filter file`` aktiviert, bzw. deaktiviert werden.
Mit ``w#automod filter add .[Dateiendung]`` und ``w#automod filter remove .[Dateiendung]`` können Dateiendungen
hinzugefügt und entfernt werden. (z.B. ``w#automod filter add .exe``)

Einladungsfilter
^^^^^^^^^^^^^^^^

Der Einladungsfilter erfasst Discord-Einladungslinks. Er kann mit ``w#automod filter invites`` aktiviert oder deaktiviert werden.

Capslockfilter
^^^^^^^^^^^^^^

Der Capslockfilter löscht Nachrichten, deren Inhalt zu einem großteil aus Großbuchstaben besteht.
Nachrichten mit weniger als zehn Zeichen werden ignoriert um das Filtern von Abkürzungen zu vermeiden.

``ẁ#automod filter caps <Wert>`` aktiviert oder deaktiviert den Capslockfilter.
``<Wert>`` ist optional, damit kannst du den den Prozentwert angeben, ab wann der Capslockfilter durchgreifen soll.
(Standardmäßig 50%)

Nachricht
^^^^^^^^^

Falls der Automod durchgreift, sendet Weemo eine Nachricht in den entsprechenden Chat. Diese Nachricht kann mit
``w#automod filter message [Nachricht]`` eingestellt werden.
Durch das Einfügen von Platzhaltern in die Nachricht, wird diese beim senden auf die Nutzer personalisiert.

.. csv-table::
    :widths: auto
    :align: left
    :header: "Platzhalter", "Beschreibung"

    "``%user%``", "Name des Nutzers / der Nutzerin"
    "``%mention%``", "Erwähnung des Nutzers / der Nutzerin"
