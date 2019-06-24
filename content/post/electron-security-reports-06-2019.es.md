---
author: "Daniell Mesquita"
title: Informes de seguridad Electron para las apps preinstaladas de Floflis
date: 2019-06-23T18:11:28-04:00
categories: ["seguridad"]
tags: ["seguridad", "informes"]
---

Hace unos días estudiaba sobre auditores de seguridad en Linux, primero comencé con la auditoría de aplicaciones de Electron.

La primera herramienta de auditoría (y actualmente la única que estoy usando) es Electronegativity por <a href="https://doyensec.com/" target="_blank">Doyensec</a>.

Electronegativity había señalado vulnerabilidades en todas las aplicaciones. No sé si son realmente vulnerabilidades o solo consejos de mejores prácticas de JS.

Los he reportado a todos los desarrolladores, y parecían escépticos, y ignoraron. Pero me comprometo a tratar de corregir las vulnerabilidades en cualquier aplicación que desarrolle para Floflis, especialmente sus aplicaciones integradas. Esa es la razón por la que eliminaré temporalmente el `HTML5 Player`, ya que se considera un navegador web: es la aplicación más sensible.

<a href="https://floflis.github.io/security/reports/06-2019/" target="_blank"> Haga clic aquí </a> para ver todos los informes, con un enlace a su issue de GitHub.
