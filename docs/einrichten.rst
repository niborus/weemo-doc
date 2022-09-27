.. warning::
    Die Dokumentation könnte an einigen Stellen nicht mehr aktuell sein, da Weemo auf Slash-Commands migriert hat. Bitte habt ein wenig Geduld, während die Dokumentation aktualisiert wird.

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

Moderations-Logbuch
-------------------

Weemo ist in der Lage, bestimmte Aktionen in einem Textkanal, dem :ref:`Modlog<modlog>`, zu loggen.
Erstellt dazu einen Kanal, der am besten nur für Logs da ist.
Nutzt dann ``/modlog settings`` zum aktivieren der Funktion.

Automatische Moderation
-----------------------

Einige Sachen kann Weemo auch von alleine Moderieren. Seht euch dazu einmal den :ref:`Automod<automod>` an.

Wichtige Befehle
----------------

Für die Moderatoren gibt es einige wichtige Befehle, die nicht eingerichtet werden müssen. 
Um eine Übersicht über diese, sowie deren Syntax zu erhalten, gebt ``/tag view modhelp`` auf dem Weemo HQ ein
oder seht euch die :ref:`Befehle für Moderator\*innen<moderation_befehle>` an.

Soziales
========

*Weemo bietet verschiede Möglichkeiten, soziale Profile aufzustellen. Dies muss jedoch jedes Mitglied für sich Persönlich einrichten.*

Das Profil [Serverübergreifend]
-------------------------------

Das Profil enthält allgemeine Informationen über euch.
Mit ``/help profile`` oder :ref:`hier<befehle_profile>` könnt ihr sehen, wie ihr es einrichtet.
Mit ``/birthday`` fügt ihr euren Geburtstag hinzu.

Splatoon 3 Karte [Serverübergreifend]
-------------------------------------

Die Karte enthält Informationen über eure Splatoon 3 Ränge.
Die Anleitung zum einrichten ist unter ``/help card`` und im Menü :ref:`befehle_card`.

Nintendo-Switch-Freundescode [Serverübergreifend]
-------------------------------------------------

Euren Freudescode kann man mit ``w#fc`` speichern und auch wieder abrufen.

Nützliches
==========

Levelrollen
-------------

Falls ihr für besondes aktive Mitglieder Rollen verteilen wollt, findet ihr bei ``/leveledroles``
und :ref:`hier<befehle_leveledroles>` mehr Informationen dazu.

Private Kanäle
--------------------

Damit euer Server :ref:`Private Kanäle<befehle_private_sprachkanaele>` nutzen kann,
müsst ihr vorher mit ``/roomcategory set [Kategorie]`` eine Kategorie für die Kanäle festlegen.

Begrüßung und Verabschiedung
----------------------------

Um Mitglieder auf dem Server automatisch zu begrüßen und zu verabschieden, nutzt ``/joinmessage`` und ``/leavemessage``.
(Siehe :ref:`joinmsg_leavemsg`)
Um einem neuen Mitglied eine Rolle zuzuweisen, nutzt ``/joinrole``. (siehe :ref:`befehle_joinrole`)

Emojiquiz
----

Weemo hat ein :ref:`Emojiquiz<emojiquiz>`.
Nutzt ``/emojiquiz`` um es auf eurem Server einzurichten oder probiert es auf dem Weemo HQ im #emojiquiz einfach mal aus.


Abschließend
============

Dies sind alle Befehle, die man einrichten muss. Viele weitere Funktionen funktionieren von vorne herein. Probiert euch einfach aus.
Bei Fragen, helfen euch die Agenten gerne.
