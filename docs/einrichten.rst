****************
Weemo einrichten
****************

.. contents:: Inhalte

Hallo und Danke, dass du dich für Weemo entschieden hast.
Im Folgenden werde ich euch zeigen, welche Einstellungen ihr machen könnt,
damit Weemo auf eurem Server optimal funktioniert.
Das ganze wird in vier Kategorien eingeteilt: **Moderation**, **Nützliches**, **Soziales** und **Prefix**.

Moderation
==========

**Falls Weemo den Server moderieren soll, ist es wichtig, dass ihr diese Einstellung vornehmt:**

Moderator\*inrolle
------------------

Im besten Fall haben eure Moderatoren bereits eine Moderator\*inrolle.
Falls nicht, legt eine neue an und weist diese all euren Moderator\*inen zu.
**w#modrole @Moderator\*inrolle** gibt allen Personen mit der Moderator\*inrolle
uneingeschränkten Zugriff auf ``ban``, ``idban``, ``unban``, ``kick`` und ``warn``.

Moderations-Logbuch
-------------------

Weemo ist in der Lage, bestimmte Aktionen in einem Textkanal zu loggen. Erstellt dazu einen Kanal,
der am besten nur für Logs da ist. Nutzt dann **w#modlog** zum aktivieren der Funktion.

Automatische Moderation
-----------------------

Einige Sachen kann Weemo auch von alleine Moderieren. Nutzt **w#automod** und **w#help automod** um einen Überblick zu erhalten.

Wichtige Befehle
----------------

Für die Moderatoren gibt es einige wichtige Befehle, die nicht eingerichtet werden müssen. 
Um eine Übersicht über diese, sowie deren Syntax zu erhalten, gebt **w#tag modhelp** ein.

Soziales
========

*Weemo bietet verschiede Möglichkeiten, soziale Profile aufzustellen. Dies muss jedoch jedes Mitglied für sich Persönlich einrichten.*

Das Profil [Serverübergreifend]
-------------------------------

Das Profil enthält allgemeine Informationen über euch.
Mit **w#help profile** könnt ihr sehen, wie ihr es einrichtet. Mit **w#bday** fügt ihr euren Geburtstag hinzu.

Splatoon 2 Karte [Serverübergreifend]
-------------------------------------

Die Karte enthält Informationen über eure Splatoon 2 Ränge. Die Anleitung zum einrichten ist unter **w#help card**

Nintendo-Switch-Freundescode [Serverübergreifend]
-------------------------------------------------

Euren Freudescode kann man mit **w#fc** speichern und auch wieder abrufen.

Nützliches
==========

Leveled Roles
-------------

Falls ihr für besondes aktive Mitglieder Rollen verteilen wollt, findet ihr bei **w#help leveledroles** mehr Informationen dazu.

Private Sprachkanäle
--------------------

Damit euer Server Private Sprachkanäle nutzen kann, müsst ihr vorher mit **w#setcategory** eine Kategorie für die Kanäle festlegen.

Starboard
---------

Um Informationen zur Einrichtung des Starboards zu bekommen, nutzt **w#help starboard**.

Begrüßung und Verabschiedung
----------------------------

Um Mitglieder auf dem Server automatisch zu begrüßen und zu verabschieden, nutzt **w#joinmsg** und **w#leavemsg**.
Um einem neuen Mitglied eine Rolle zuzuweisen, nutzt **w#joinrole**.

Quiz
----

Weemo hat ein Emojiquiz. Nutzt **w#quiz** um es auf euerm Server einzurichten oder probiert es auf dem Weemo HQ im #emojiquiz einfach mal aus.

Präfix
======

Um einen anderen Präfix als ``w#`` zu verwenden, nutzt ``w#prefix <neuer Präfix>``.
Aktuell werden nur folgende Prefixe unterstützt:
``w#``
``-``
``_``
``+``
``*``
``/``
``%``
``.``
``#``
``!``
``?``
``!!``
``??``
``--``
``++``
``//``
``?!``

Abschließend
============

Dies sind alle Befehle, die man einrichten muss. Viele weitere Funktionen funktionieren von vorne herein. Probiert euch einfach aus.
Bei Fragen, helfen euch die Agenten gerne.
