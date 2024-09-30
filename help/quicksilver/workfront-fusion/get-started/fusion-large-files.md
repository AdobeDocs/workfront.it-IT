---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Utilizzo di file di grandi dimensioni in Adobe Workfront Fusion
description: Il supporto per file di grandi dimensioni è attualmente disponibile per i connettori Workfront e HTTP.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: 630467ca64281df0b257dae8cc5c6edc55ae56ad
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# Utilizzo di file di grandi dimensioni in Adobe Workfront Fusion

Alcuni connettori Fusion possono supportare file di dimensioni superiori al limite di 1 GB.

## Connettori che supportano file di grandi dimensioni

Il supporto per file di grandi dimensioni è attualmente disponibile per i seguenti connettori:

* Workfront
* HTTP

## Effetto della dimensione file di grandi dimensioni sul tempo di esecuzione dello scenario

Il caricamento, il download o l&#39;elaborazione di file di grandi dimensioni nello scenario Fusion potrebbe richiedere del tempo. Anche se non esiste un limite alla dimensione del file, il tempo di esecuzione dello scenario è limitato a 40 minuti. Pertanto, se i file di grandi dimensioni fanno durare l’esecuzione più di 40 minuti, lo scenario non riesce.

Il tempo di esecuzione di uno scenario può essere influenzato anche dalle dimensioni dello scenario, dalla complessità del modulo e dalla velocità di rete. Pertanto, si consiglia di considerare questi aspetti degli scenari quando si utilizzano file di grandi dimensioni.


<!--
## Connectors that do not support large files

Some Fusion connectors do not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

The following connectors do **not** support large files. 

* Archive
* Box
* Convert
* CSV
* Datastores
* Flow control
* FTP
* JSON
* JWT
* Markdown
* Math
* Microsoft Word templates
* MIME
* Microsoft SQL
* SFTP
* Adobe Acrobat Sign
* SOAP
* Tools
* XML

If a connector is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.-->






<!--## Connectors that support large files

The following connectors support large files.

Workfront
HTTP
Webhooks
Salesforce
Microsoft Email
Workfront Proof
AEM Assets
Email
Slack
Jira
Microsoft Excel
SharePoint
Frame.io
Adobe PDF Services
Marketo
Azure Devops 
Google Email
Jira Server
Google Sheets
Microsoft OneDrive
ServiceNow 
AWS S3
Bynder
OneDrive Business
Adobe Authenticator
Google Drive
Microsoft Dynamics
Google Docs
NetSuite
Airtable
Azure AD
QuickBase 
Adobe Target
Adobe Campaign Classic
Microsoft Calendar
Workfront Planning
HubSpot CRM  
DropBox
Cloud Convert
Egnyte
Adobe Firefly
OpenAI / Chat GPT
Allocadia
Cvent
GitLab 
Google Team Drive
Google Calendar
Workfront SDL Managed Translation
Widen
Workfront Boards
Google Slides
Qualtrics
Microsoft Power BI
Adobe Photoshop
Anaplan
DocuSign 
MariaDB
Adobe Creative Cloud Libraries
Figma
AEM Forms
Datadog
GitHub 
Google Forms
Adobe I/O Events
Trello
Workday
Adobe Journey Optimizer
Adobe Lightroom









If a file is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

-->