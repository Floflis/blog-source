---
author: "Daniell Mesquita"
title: Die Sicherheitsberichte von Electron für die vorinstallierten Floflis-Apps
date: 2019-06-23T18:11:28-04:00
categories: ["sicherheit"]
tags: ["sicherheit", "berichte"]
---

Vor einigen Tagen habe ich mich mit Sicherheitsprüfern unter Linux befasst und zunächst mit der Prüfung von Electron-Apps begonnen.

Das erste Prüfungstool (und derzeit das einzige, das ich verwende) ist die Electronegativity von <a href="https://doyensec.com/" target="_blank">Doyensec</a>.

Die Elektronegativität wies in allen Apps auf Schwachstellen hin. Ich weiß nicht, ob es sich wirklich um Sicherheitslücken oder nur um Tipps für bewährte Vorgehensweisen bei JS handelt.

Ich habe sie allen Entwicklern gemeldet, und sie wirkten skeptisch und ignoriert. Aber ich bin fest entschlossen, Schwachstellen in jeder App zu beheben, die ich für Floflis entwickle, insbesondere in den integrierten Apps. Aus diesem Grund werde ich `HTML5 Player` vorübergehend entfernen, da es sich um einen Webbrowser handelt. Dies ist die sinnvollste Art von App.

Aufgrund der schlechten <a href="https://github.com/fabiospampinato/noty/issues/10" target="_blank">erhaltenen Antwort</a> entfernt Floflis `noty` als installierte App.

<a href="https://floflis.github.io/security/reports/06-2019/" target="_blank">Klicken Sie hier</a>, um alle Berichte mit einem Link zu ihrem GitHub-Problem anzuzeigen.
