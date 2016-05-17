# Roadmap für die Weiterentwicklung des Kurses

Basierend auf den Kommentaren der Teilnehmern und meinen eigenen Ideen, werde ich dokumentieren, welche nächsten Lektionen in den Kurs eingefügt werden.

## Lektionen für den Abschnitt Tips & Tricks

GitHub hält an einige Stellen so seine Überraschungen für einen bereit. Daher verrate ich dir in diesem Abschnitt die wichtigsten Tips & Tricks.

### Tags - Von Visual Studio bis zum Release auf GitHub 

Auf GitHub gibt es einen eigenen Bereich für Releases. Dieser wird "gesteuert" über Tags die du in Git setzt. In dieser Lektion zeige ich dir wie du Tags erstellst, wie du sie aus Visual Studio nach GitHub bekommst und wie du dann in GitHub das ganze überarbeiten kannst.

### Two Factor Authentication - Visual Studio kann das auch

Nach einigen Problemen mit gehackten Accounts hat GitHub schon vor einiger Zeit eine Two Factor Authentication eingeführt. Damit brauchst du nicht nur ein Passwort, sondern du bekommst auch noch einen Code auf dein Smartphone geschickt, den du dann bei der Anmeldung eingeben musst. 

Damit du dich auch mit Visual Studio anmelden kannst, wenn du diese Funktionalität eingeschaltet hast, zeige ich dir in dieser Lektion die notwendigen Schritte. 

Hier die notwendingen Schritte: http://www.anilsezer.com/connecting-github-from-visual-studio-after-twofactor-authentication-enabled

### Gute Commit-Messages

Diese Lektion sollte vielleicht besser in den Git-Kurs. Vielleicht kann ich sie aber auch in beiden Kursen einfach verwenden. Hier die passenden Quellen dazu:

 - http://www.slideshare.net/TarinGamberini/commit-messages-goodpractices
 - https://wiki.openstack.org/wiki/GitCommitMessages
 - http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html

Außerdem sollte ich im Screencast dann Beispiele von guten Commit-Messages zeigen. Auch würde mich interessieren, wie ich die auf der Kommandozeile oder in VS so schreiben kann wie unten beschrieben.

Gute Commit-Messages sind die Grundlage um aus der Historie eines Projektes schlau zu werden. Du brauchst sie also selber, wenn du:

 - dir gewisse Änderungen nochmals anschauen willst,
 - Änderungen am Quellcode auch in einigen Wochen, Monaten oder Jahren noch verstehen willst,
 - wissen möchtest wann Funktionalitäten integriert wurden,
 - verstehen möchtest warum und wie Funktionalitäten integriert wurden,
 - aus deinem Vorgehen lernen willst.

Eine Commit-Message besteht immer aus mindestens der ersten Zeile. Dabei sollte diese folgende Kriterien erfüllen: 

 - Ist nicht länger als 50 Zeichen
 - Endet nicht mit einem Punkt
 - Gibt einen ersten Überblick über die Änderung

Die erste Zeile einer Commit-Message wird üblicherweise als "Betreff" in einer Mail verwendet, die automatisch von GitHub bzw. Git verschickt wird.

Die darauf folgende zweite Zeile sollte leer sein. Danach können weitere Abschnitte folgen, die eine detaillierte Beschreibung enthält. Dabei sollten die einzelnen Zeilen in diesem Abschnitten nicht mehr als 72 Zeichen haben. Inhaltlich wird dabei auf die folgenden Aspekte eingegangen:

 - Das ursprüngliche Probleme
 - Warum die Änderung im Commit gemacht wurde
 - Einschränkungen bzw. Probleme die der neue Code noch hat

Sofern im Projekt externe Ressourcen verwendet werden (z.B. ein Werkzeug zum Bug-Tracking), dann können noch die entsprechenden Verweise (z.B. Id des gelösten Problems aus dem Bug-Tracking) in die Message integriert werden.

Eine Commit-Message sollte im Imperativ, also der Befehlsform, geschrieben werden. Dieses wird bei automatischen Aktionen (z.B. einem merge) auch so gemacht und garantiert eine einheitliche Historie.

### GitHub Issues in anderen Tools

Neben der Integration mit Visual Studio, kannst du die Issues aus GitHub in vielen anderen Tools verwenden. Darunter die folgenden:

 - Trello - Projektmanagement / Produktivitätstool in der Cloud. Egal ob agile Softwareentwicklung oder Kanban, mit Trello und der GitHub Integration hast du immer einen guten Überblick was gerade in deinem Projekt geschieht. Insbesondere bei Webentwicklern ist Trello recht beliebt.
 - Everhour - Die "Stempeluhr" für GitHub. Mit Everhour kann das komplette Entwicklungsteam die aktuell angefallenen Aufwände gegen GitHub Issues buchen und auch Schätzungen machen und somit in die Planung einsteigen. Dabei brauchen die Entwickler die GitHub-Oberfläche nicht zu verlassen.
 - ZenHub - Ein KanBan-Board basierend auf den Issues in GitHub. Es ist also eine Visualisierung der bestehenden Issues und nichts wird umgewandelt oder so.
 - HuBoard - Scheint ähnlich wie ZenHub zu sein. Wo liegen die Unterschiede? Was sollte besser verwendet werden?

Macht es Sinn die einzelnen Integrations genauer zu betrachten und daraus jeweils einen eigenen kleinen (kostenlosen?) Kurs zu machen?

https://github.com/integrations

### Issue-only Repository

https://help.github.com/articles/issues-only-access-permissions/

### GitHub Projekt-Graphs - Was passiert in (d)einem Projekt?

Eine Verwendung der Graphs-Funktionalität habe ich dir bereits erklärt. In dieser Lektion werde ich dir genauer zeigen, welche Informationen dir GitHub über dein eigenes, aber auch über Projekte von anderen bereitstellt.

 - Traffic - Das "Analytics" für dein Projekt. Im Bereich "Traffic" siehst du wie andere Benutzer mit deinem Projekt interagieren. Neben der Information wie viele Benutzer dein Projekt geklont haben und wie viele Besucher / Views deine Projektseite hat, bekommst du hier noch weitere Details. So siehst du beispielsweise woher die Benutzer hauptsächlich kommen und welche Inhalte sie besonders interessant finden. Alle diese Information bekommst du nur für deine eigenen Projekte!
 - Punch Card - Lass dir zeigen wann Leute besonders aktiv an einem Projekt arbeiten. Die "Punch Card" (engl. für Lochkarte) zeigt an an welchen Wochentagen und zu welcher Uhrzeit die Commits gemacht werden. Dies ist eine gute Möglichkeit herauszufinden ob bei einem Projekt eine Firma die Zügel in der Hand hat, oder doch eher Personen die es in Ihrer Freizeit machen. ( http://openmymind.net/How-Meaningful-Do-You-Find-Github-Punchard/ )
 - Network - ???

### Fast Forward

Ist eines der häufigen Probleme bei einem Sync. Ist jedoch die Frage ob ich das wirklich in diesem Kurs oder besser im Git Kurs besprechen sollte.

### Bei Problemen mit GitHub in Visual Studio - Eingabeaufforderung benutzen!

Manchmal passiert es, dass gewisse Aktionen einfach nicht laufen wie sie sollen. So kommt es manchmal vor, dass du einen Branch nicht aus Visual Studio nach GitHub bekommst, oder auch das andere Dinge nicht funktionieren.

Dann ist es wichtig, dass du dir mehr Informationen über das aktuelle Problem besorgen kannst. Dafür gibt es auch unter Windows die Eingabeaufforderung. Diese ist jedoch erstmal nicht so konfiguriert, dass du einfach git-Befehle ausführen kannst.

In dieser Lektion zeige ich dir erste Schritte was du bei Problemen machen kannst und vor allem wie du die Eingabeaufforderung installierst und vorbereitest.
