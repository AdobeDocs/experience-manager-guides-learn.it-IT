---
title: API REST per registrare un connettore di origine dati
description: Scopri l’API REST per registrare un connettore di origine dati
source-git-commit: 880cd344ceb65ea339be699ebcad41c0d62e168a
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 0%

---

# API REST per registrare un connettore di origine dati {#id236LG0Y0CXA}

La seguente API REST consente di registrare un connettore dell’origine dati.

## Registrare un connettore di origine dati

Metodo di GET che registra un connettore di origine dati.

**URL richiesta**:
`http://server:port/bin/guides/v1/konnect/config/register?path=<uploaded file path>`

**Parametro**: |Nome|Tipo|Obbligatorio|Descrizione| ----|----|--------|-----------| |`path`|String|Yes|Stringa che punta a un percorso nell&#39;archivio AEM. Può essere un percorso in `/content/dam or /var/dxml`.|

**Esempio**:\
`http://host:4502/bin/guides/v1/konnect/config/register?path=/var/dxml/konnect/jira.json`
