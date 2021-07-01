+++
title = "Eigenes Game Teil 1"
date = "2021-05-27"
draft = false
pinned = false
tags = ["Projekt", "Construct3", "Lernen"]
image = "bild_2021-05-27_110004.png"
description = "Ich versuche ein eigenes \"Beat em Up\" Game zu erstellen."
footnotes = "construct.net"
+++
Ich wollte schon sehr lange ein eigenes Game erstellen. Da ich ziemlich faul bin lernte ich aber nie eine nötige Programmiersprache so wie "C#" oder "C++". Da stieß ich auf eine Website namens Construct 3 (Link in Fußnote). Mit der gratis Version dieses Programmes ist es möglich ohne Programmiersprachenkenntnis ein game zu programmieren. Als Tutorial fand ich ein YouTube Video, dass zwar für ein Plattformer Spiel (so wie Super Mario) ist, aber für mich reichte dies. (https://www.youtube.com/watch?v=83Vi4AMJJ1o&t=0s) Ich entschied mich für ein "Beat `em up" Game. Das heißt, 2 Charaktere die aus einer Seitenansicht gegen einander kämpfen. Ich entschied mich dafür, weil ich dachte, dass, das nicht allzu schwierig sein sollte..... Zuerst zeichnete ich meinen Charakter, der bis jetzt nur ein Strichmännchen ist. Aber das kann ich mit allem ersetzen, was ich will. Ich musste auch alle einzelnen Bewegungsschritte des Charakters zeichnen. 

![Alle Animationsframes (Eigentlich nur Place Holders)](player-sheet0.png)

Dazu musste ich noch eine sogenannte Hit Box um den Charakter legen, das ist dann die Form, in welcher der Computer den Charakter sieht. Also eigentlich die "wahre" Form des Charakters, hinter dem Skin.

![Die Orangen Punkte sind die Eckpunkte des Hit Box Gitternetzes. Die Bilder unten zeigen die Schlag Animation.](hitbox.png)

Darauffolgend kopierte ich den Charakter und färbte ihn Weiß für den zweiten Spieler.

![Ich gestaltete noch eine Landschaft und setzte ein vorläufiges Hintergrundbild ein.](screenshot-2021-05-27-110953.png)

Dann ging es ans Skript, also an die Funktionen. Das heißt, dort sage ich was passiert, wenn ich welche Taste drücke. Im Endeffekt emuliere ich mit WASD die Pfeiltasten. Wie man im unteren Bild sehen kann, benötigte ich keinen Code, sondern konnte einfach die Funktionen auswählen. Z.B "Wenn ich D drücke, dann bewege dich nach rechts, schaue nach rechts und spiele die gehen Animation ab." 

![Das ganze Skript für einen Charakter.](skript.png)

Danach begann ich einzuprogrammieren, dass bei einem Treffer Schaden zugefügt wird. Dazu habe ich die Health-bar selber gezeichnet und das mit 17 Stufen, mit dem Ziel dass man 17 Schläge braucht, um den Gegner zu besiegen. Das erste Problem war, dass bei einem Schlag beide gleich viel Schaden nahmen. Da fand ich den Fehler im Skript und merzte ihn aus. Beim Test aber, funktionierte es immer noch nicht. Ich merkte, dass die rechte Health-Bar durchs kopieren der Linken, mit der verknüpft war. Also musste ich eine neue Instanz machen, und dann die 17 Frames, Frame by Frame kopieren und einfügen. Als dann diese Funktion funktionierte, fiel mir auf, dass man nur etwa 6-9 Schläge benötigte um den Gegner zu besiegen. 

Dagegen habe ich noch keine Lösung gefunden.