---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Cerca [!DNL Adobe Workfront] elementi da [!DNL Slack]
description: È possibile cercare [!DNL Adobe Workfront] elementi da [!DNL Slack], se nell'istanza di Slack è installata l'app [!DNL Workfront].
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
TQID: 'https://experienceleague.adobe.com/JulYq173XQa6mG93qzUwfBDn4TPVEafD2OVpcIAXxi8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
subfeature_v2:
  - id: e4fedd42-4a54-4109-859f-13c7f0366a72
    internal-label: Adobe Workfront for Slack
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 19%
---
# Cerca [!DNL Adobe Workfront] elementi da [!DNL Slack]

È possibile cercare [!DNL Adobe Workfront] elementi da [!DNL Slack], se nell&#39;istanza di [!DNL Slack] è installata l&#39;app [!DNL Workfront].

Per ulteriori informazioni sulla configurazione di [!DNL Workfront] con [!DNL Slack], vedere [Configure [!DNL Adobe Workfront] for [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Qualsiasi</p>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di poter cercare [!DNL Workfront] elementi da [!DNL Slack], è necessario

* Configura [!DNL Workfront] per [!DNL Slack]\
   Per istruzioni sulla configurazione di [!DNL Workfront for Slack], vedere [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Cerca [!DNL Workfront] elementi da [!DNL Slack]:

1. Accedi all&#39;istanza [!DNL Slack] e accedi a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedere la sezione &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare uno dei seguenti comandi nel campo del messaggio:

   `/workfront search <keyword>`

   Oppure

   `/wf search <keyword>`

   >[!NOTE]
   >
   >I comandi distinguono tra maiuscole e minuscole. La parola chiave non fa distinzione tra maiuscole e minuscole e deve essere immessa senza parentesi quadre o virgolette.

1. Nel campo visualizzato, selezionare un tipo di oggetto tra i seguenti:

   * Progetto
   * Attività
   * Problema
   * Rapporto
   * People
   * Modello
   * Documento
   * Portfolio
   * Programma
   * Dashboard
   * Azienda
   * Nota

     È possibile selezionare un solo tipo di oggetto alla volta.\
      Viene visualizzato un elenco di elementi che corrispondono ai criteri di ricerca.

1. Fare clic sul nome di un elemento per aprirlo in [!DNL Workfront] in una nuova scheda del browser.
