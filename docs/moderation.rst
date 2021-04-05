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
